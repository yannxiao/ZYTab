## ZYTab
依赖jQuery，支持CMD、AMD。每个Tab使用`data-zt`属性指定对应的内容，对应关系非常明确。

### 基本用法
```javascript
new ZYTab({
    // Tab选择器，必须
    selector: '',
    // 默认Tab，可选，默认为第一个
    defTab: '',
    // 事件类型，可选，默认为 click
    event: '',
    // Tab选中后的样式，可选，默认为 zt-active
    activeClass: '',
    // 该方法默认为切换选中的Tab的样式，可根据需求重写
    setTab: function() {},
    // 该方法默认为显示选中的Tab内容，可根据需求重写
    setBody: function() {},
    // 可以直接这样扩展自定义方法，上下文为当前新建的对象
    yourFunction: function() {}
});

```