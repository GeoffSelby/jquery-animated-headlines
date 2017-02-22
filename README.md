# jQuery Animated Headlines

Animated headlines, with interchangeable words that replace one another through CSS transitions.

## Installation

### npm

```bash
npm install jquery-animated-headlines
```

### npm
Coming soon.

### Default Usage

Include the css in your head.
```html
<link rel="stylesheet" src="dist/css/jquery.animatedheadline.css">
```

Use the following markup.
```html
<div class="selector">
    <h1 class="ah-headline">
        <span>My favorite food is</span>
        <span class="ah-words-wrapper">
            <b class="is-visible">pizza</b>
            <b>sushi</b>
            <b>steak</b>
        </span>
    </h1>
</div>
```

Finally, initialize the plugin.
```html
<script src="dist/js/jquery.animatedheadline.min.js"></script>
<script>
    $(function() {
        $('.selector').animatedHeadline();
    })
</script>
```

## Advanced Usage

The plugin provides multiple options to customize the animation type and delay.
```html
<script>
    $(function() {
        $('.selector').animatedHeadline({
            animationType: 'type'
        });
    })
</script>
```

## Options

It is recommended to use the default delay options. Because of this, I won't list them below. See `src/js/jquery.animatedheadline.js` for a complete list of options.

<table>
    <tr>
        <th>Name</th>
        <th>Type</th>
        <th>Default</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>animation-type</td>
        <td>string</td>
        <td>'rotate-1'</td>
        <td>Type of animation used. Options: 'rotate-1', 'rotate-2', 'rotate-3', 'type', 'loading-bar', 'slide', 'clip', 'zoom', 'scale', and 'push'</td>
    </tr>
</table>

## License

jQuery Animated Headlines is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).