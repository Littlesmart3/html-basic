### < form > 元素

所有HTML表单都以一个< form >元素开始：

```
<form action="/my-handling-form-page" method="post">

</form>
```

这个元素正式定义了一个表单。就像< div >或 < p > 元素，它是一个容器元素，但它也支持一些特定的属性来配置表单的行为方式。它的所有属性都是可选的，但实践中最好至少要设置`action`属性和`method`属性。

- `action` 属性定义了在提交表单时,应该把所收集的数据送给谁(/那个模块)(URL)去处理。.
- `method` 属性定义了发送数据的HTTP方法(它可以是“get”或“post”).



##### < button >元素

我们的表格已经快准备好了，我们只需要再添加一个按钮，让用户在填写完表单后发送他们的数据。这是通过使用 [`元素完成的。在 `</form>这个结束`标签上方添加以下内容：

```
<div class="button">
  <button type="submit">Send your message</button>
</div>
```

您会看到< button >元素也接受一个 `type`属性，它接受`submit`, `reset`或者 `button` 三个值中的任一个。

- 单击 `type` 属性定义为 `submit` 值(也是默认值)的按钮会发送表单的数据到< form >元素的`action` 属性所定义的网页。
- 单击 `type` 属性定义为 `reset` 值的按钮 将所有表单小部件重新设置为它们的默认值。从用户体验的角度来看，这被认为是一种糟糕的做法。
- 单击 `type` 属性定义为 `button` 值的按钮……不会发生任何事！这听起来很傻，但是用JavaScript构建定制按钮非常有用。 