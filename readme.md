# jQuery Tabber
## Structure
```html
<div id="tabber">
	<div class='tabber-selectors'>
		<ul>
			<li>
			</li>
		</ul>
		<a class='tabber-anchor active' href='javascript:;'>Tab 1</a>
		<a class='tabber-anchor' href='javascript:;'>Tab 2</a>
		<a class='tabber-anchor' href='javascript:;'>Tab 3</a>
	</div>
	<div class='tabber-contents'>
		<div class='tabber-content active'>Contents accroding to Tab 1</div>
		<div class='tabber-content'>Contents accroding to Tab 2</div>
		<div class='tabber-content'>Contents accroding to Tab 3</div>
	</div>
</div>
```
note: class `tabber-selectors` and `tabber-contents` is required.
## Usage
include *jquery.tabber.js* after jQuery Library

`<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>`  
`<script src='jquery.tabber.js' type='text/javascript'></script>`
### Initial
`
$('#tabber').tabber();
`

## Options

```
$('#tabber').tabber({  
	'anchor': '.tabber-anchor',  
	'content' : '.tabber-content'	
});
```

## Styling

jquery.tabber does not include any styling, you shoud do it by your self.  
see essensial examples below: (sass)
```
//Basic Styling
#tabber {
	.tabber-selectors {
		ul {
			margin: 0;
			padding: 0;
			list-style-type: none;
			font-size: 0;
			li {
				display: inline-block;
				vertical-align: middle;
			}
		}
		a {
			font-size: 1rem;
			display: block;
			color: $white;
			padding: .8em 1.6em;
		}
		.tabber-anchor {
			background-color: $blue;
			&:hover, &.active {
				background-color: darken($blue, 15%);
			}
		}
	}
}
.tabber-contents {
	padding: 1em;
	box-sizing: border-box;
	background-color: $white;
	.tabber-content {
		display: none;
		&.active {
			display: block;
		}
	}
}
```
**anchor (selector)**
>*String*

**content (selector)**
>*String*


---
Any contribution is welcome.
chiang@walkingho.me