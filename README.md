# An DonatePay.ru Itegration

Right now it's support only donate event.

# Installation

- install by `npm i donatepay --save`
- take widget token from http://donatepay.ru (not API)

# Usage

Your app:

```javascript
const DonatePay = require('donatepay')
const donatePay = new DonatePay(*/token from donatepay.ru/*)
donatePay.onDonate(callback => console.log(callback))
```

Example callback object:

```
{ username: 'DonatePay',
  amount: 1337,
  message: 'Message of Donation' }
```