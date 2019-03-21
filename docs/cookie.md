
# Cookie 文档

[MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/Document/cookie)

## 定义

cookie 是一个键值对形式的字符串。

## 设置

```js
document.cookie = newCookie;
```

> 用这个方法一次只能对一个cookie进行设置或更新。


**格式**：`key=value;path=/` value 值可以用 encodeURIComponent() 来保证它不包含任何逗号、分号或空格(cookie值中禁止使用这些值).

**可选参数**：

  + `;ptah=ptah` 默认当前路径
  + `;domain=domain` 默认当前域名
  + `;max-age=max-age-in-seconds` 设定多少秒后过期 (例如一年为60*60*24*365)
  + `;expires=date-in-GMTString-format` 如果没有定义，cookie会在对话结束时过期
  + `;secure` cookie只通过https协议传输

## 操作库

[js-cookie](https://github.com/js-cookie/js-cookie)
