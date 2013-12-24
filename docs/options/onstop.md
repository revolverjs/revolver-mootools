# onStop

**Type**: `Function`, **Default**: `function(){}`

This is a callback that you can pass through the options object to the constructor. Internally, it is registered as a listener to the [stop](../events/stop.md) event using the [on](../methods/on.md) method. The `this` variable inside the callback is equal to the Revolver instance.

```javascript
var slider =  new Revolver($('.slides'), {
  onStop: function() {
    // this == slider
  }
});
```

**Source Refs**: [[48](../../coffee/revolver.coffee#L48), [68](../../coffee/revolver.coffee#L68)]