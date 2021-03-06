---
id: 587d7b7e367417b2b2512b21
title: 使用多个三元运算符
challengeType: 1
videoUrl: 'https://scrimba.com/c/cyWJBT4'
forumTopicId: 301179
dashedName: use-multiple-conditional-ternary-operators
---

# --description--

在之前的挑战中，你使用了一个条件运算符。你也可以将多个运算符串联在一起以检查多种条件。

下面的函数使用 if，else if 和 else 语句来检查多个条件：

```js
function findGreaterOrEqual(a, b) {
  if (a === b) {
    return "a and b are equal";
  }
  else if (a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```

上面的函数使用条件运算符写法如下：

```js
function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" 
    : (a > b) ? "a is greater" 
    : "b is greater";
}
```

即便如此，应谨慎使用多个三元运算符，因为在没有适当缩进的情况下使用多个三元运算符可能会使您的代码难以阅读。 例如：

```js
function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" : (a > b) ? "a is greater" : "b is greater";
}
```

# --instructions--

在 checkSign 函数中使用多个条件运算符来检查数字是正数 ("positive")、负数 ("negative") 或零 ("zero")。

# --hints--

`checkSign`应该使用多个条件运算符。

```js
assert(/.+?\s*?\?\s*?.+?\s*?:\s*?.+?\s*?\?\s*?.+?\s*?:\s*?.+?/gi.test(code));
```

`checkSign(10)`应该返回 "positive" 注意，结果对大小写敏感。

```js
assert(checkSign(10) === 'positive');
```

`checkSign(-12)`应该返回 "negative" 注意，结果对大小写敏感。

```js
assert(checkSign(-12) === 'negative');
```

`checkSign(0)`应该返回 "zero" 注意，结果对大小写敏感。

```js
assert(checkSign(0) === 'zero');
```

# --seed--

## --seed-contents--

```js
function checkSign(num) {

}

checkSign(10);
```

# --solutions--

```js
function checkSign(num) {
  return (num > 0) ? 'positive' : (num < 0) ? 'negative' : 'zero';
}
```
