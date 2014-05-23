# &lt;web-font&gt;

Web Component using Polymer that creates a font tag to load web fonts. You know, [like olden times](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/font)...

The font tag is meant to be used before the css link tags to trigger the font loading before the styles. This could improve the performance of loading web fonts.

Web fonts are loaded using the [FontFace](http://dev.w3.org/csswg/css-font-loading/) interface. If ```FontFace``` isn’t available as a JavaScript API, a regular ```font-face``` style will be included (to the DOM) as a fallback. This might not have any performance boost but at least the font will load...


## Examples

* [Sample page](http://rawgit.com/makesites/web-font/master/example.html).


## Install

Using bower:
```
bower install web-font
```


## Usage

1. Import Web Components' polyfill:

```html
<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.2.3/platform.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.2.3/polymer.js"></script>
```

2. Import Custom Element:

```html
<link rel="import" href="bower_components/web-font/component.html">
```

3. Start using it!

```html
<font src="/url/to/my/font.woff"></font>
```

## Options

For now only ```src``` and ```family``` are supported. As support for the CSS Font Loading Module improves more attributes may be added, for example:

* unicode-range



## Credits

Initiated by Makis Tracend ( [@tracend](http://github.com/tracend) )

Distributed through [Makesites.org](http://makesites.org)


## License

Released under the [MIT License](http://makesites.org/licenses/MIT)
