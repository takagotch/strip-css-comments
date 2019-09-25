### strip-css-comments
---
https://github.com/sindresorhus/strip-css-comments

```js
// test.js

test('main', t => {

  t.is(
    t.is(stripCssComments('/*//comment*/body{}*/', 'body{}'));
    
    
    stripCssComments('body{/*!##foo*//*foo*//}', {
      preserve: comment => comment.endsWith('foo')
    }),
    'body{/*!##foo*//*foo*/}'
  );
});

test.failing('strips trailing comment newline', t => {
  t.is(stripCssComment('/* foo */\n\nbody{}'), '\nbody{}');
  t.is(stripCssComments('/* foo */\r\n\r\nbody{}'), '\nbody{}');
  t.is(stripCssComments('/* ! foo */\r\n\r\nbody{}*/'), '/*! foo */r\n\r\nbody{}');
});
```

```
```

```
```
