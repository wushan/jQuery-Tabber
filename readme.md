# jQuery Tabber
## Structure
```html
<div id="#tabber">
	<div class='tabber-selectors'>
		<a class='tabber-anchor' href='javascript:;'>Tab 1</a>
		<a class='tabber-anchor' href='javascript:;'>Tab 2</a>
		<a class='tabber-anchor' href='javascript:;'>Tab 3</a>
	</div>
	<div class='tabber-contents'>
		<div class='tabber-content'>Contents accroding to Tab 1</div>
		<div class='tabber-content'>Contents accroding to Tab 2</div>
		<div class='tabber-content'>Contents accroding to Tab 3</div>
	</div>
</div>
```

## Initial
`
$('#tabber').tabber();
`

## Options

`
$('#tabber').tabber({
	'anchor': '.tabber-anchor',
	'content' : '.tabber-content'	
});
`
### anchor (selector)
>*String*

### content (selector)
>*String*


---
>Any contribution is welcome.
>chiang@walkingho.me