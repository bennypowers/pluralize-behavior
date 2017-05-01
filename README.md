# \<pluralize-behavior\>

Simple Polymer behavior that wraps `pluralize` as `pluralize`

## Usage

Import the behavior.

```html
<link rel="import" href="../pluralize-behavior/pluralize-behavior.html">
```

Mix the behavior into your element.
```html
<script>
  Polymer({
    is: 'my-element',
    behaviors: [PolymerElements.PluralizeBehavior],
  });
</script>
```

Use it imperatively or in binding annotations:

```html
<span>Value: [[number]] [[pluralize('thing', number)]]</span>
```

```js
myMethod: function() {
  return `You have ${this.value} ${this.pluralize('item', this.value)}`;
}
```
