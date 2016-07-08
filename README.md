# mdtest

## 目录

- [测试中文 2016](#测试中文-es2016)

```js
it('should pass object with correct values to save', function() {
  var save = sinon.stub(Database, 'save');
  var info = { name: 'test' };
  var expectedUser = {
    name: info.name,
    nameLowercase: info.name.toLowerCase()
  };

  setupNewUser(info, function() { });

  save.restore();
  sinon.assert.calledWith(save, expectedUser);
});
```

## 测试中文 ES2016

测试一下，哈哈~

## Emphasis

*This text will be italic*

_This will also be italic_

~~This text will be crossed~~

**This text will be bold**

__This will also be bold__

_You **can** combine them_

## Lists

### Unordered

- Item 1
- Item 2
  - Item 2a
  - Item 2b

### Ordered

1. Item 1
2. Item 2
3. Item 3
   * Item 3a
   * Item 3b

## Images

Markdown Logo: ![logo][logo]

[logo]: http://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "logo"

## Links

http://github.com - automatic!
[GitHub](http://github.com)

## Blockquotes

As Kanye West said:

> We're living the future so
> the present is our past.

## Inline code

This is an inline code: `var example = true`

## Block code

```
console.log('Hello world!')
```

```js
console.log('Hello world!')
```

## Tables

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

## Emoji

:sparkles: :camel: :boom:

## HTML

<div>This is a html code.</div>
