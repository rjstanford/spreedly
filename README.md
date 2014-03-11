spreedly
========

A simple JS wrapper to Spreedly
-------------------------------

Its really quite silly that this isn't provided out of the box.  To use it, include the JS in your webpage
and call it thusly:

```javascript
Spreedly.tokenize({
  environmentKey: 'XXXXXXXXXXXXXXXXXXXXXXXXXXXX',
  firstName: 'Bob',
  lastName: 'Smith',
  number: '4111111111111111',
  month: 12,
  year: 2017,
  cvv: '123',
  callback: function(token) {
    alert('I tokenized a payment! Woot! ' + token);
  },
  error: function() {
    alert('Something went horribly wrong.');
  }
});
```
