---
tags:
  - practice
permalink: false
---

Константы в современном JS используют чаще, чем переменные. В большинстве случаев, значение переменной устанавливается только один раз. Хорошей практикой считается объявлять такие переменные через `const` и писать название переменной в camelCase, чтобы подчеркнуть этот факт:

```js
for (let i = 0; i < users.length; ++i) {
  const user = users[i]
  printUserInfo(user)
}
```

Используй `CAPS_WITH_UNDER` формат именования, если нужно объявить константу, которая хранит важное значение для программы: количество элементов на странице по умолчанию, формат даты, максимальное количество заказов и т.д.

```js
const ITEMS_PER_PAGE = 25

for (let i = 0; i < products.length && i < ITEMS_PER_PAGE; i++) {
  printItem(products[i])
}
```