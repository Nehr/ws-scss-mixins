# Websquid SCSS Mixins

Hello! I have no idea how you found this, but you're more than welcome to use this. I've made this to easier import my own small SCSS mixins, helpers and such between my projects.

## How to use

To use the mixins import the **main.scss**-file in your project like this:

```javascript
@import "~@downehr/ws-scss-mixins/main.scss";
// or you may have to import it like this
@import "node_modules/@downehr/ws-scss-mixins/main.scss";
```

## Breakpoints (screen size media queries)

### All breakpoint sizes

|class name| size |
|--|--|
| **ws-sm** | 576px |
| **ws-md** | 768px|
| **ws-lg** | 992px|
| **ws-xl** | 1200px|
| **ws-xxl** | 1400px|

### Example

```scss
p {
	// Default font size for 0< screen size
	font-size: 1.3rem;
	line-height: 1.125;

	@include  ws-md {
		// 768px and above
		font-size: 1.8rem;
	}

	@include  ws-lg {
		// 992px and above
		font-size: 2rem;
	}
}
```
