# Kickoff Snippets for Sublime Text

Use these snippets if you use the [Kickoff framework](https://github.com/tmwagency/kickoff/) & [Sublime Text](http://sublimetext.com)

* [Kickoff demos](http://tmwagency.github.io/kickoff/demos/)

## How to install

If you experience problems or editor crashes please [fill an issue](https://github.com/sergeche/emmet-sublime/issues).

With [Package Control](http://packagecontrol.io):

1. Run “Package Control: Install Package” command, find and install `Kickoff Snippets` plugin.
2. Restart ST editor (if required)

Manually:

1. Clone or [download](https://github.com/tmwagency/Kickoff-snippets/archive/master.zip) git repo into your packages folder (in ST, find Browse Packages... menu item to open this folder)
2. Restart ST editor (if required)

##### Tab trigger for all items: 'ko' &#8677;

## HTML
[Reference](https://github.com/tmwagency/Kickoff-snippets/tree/master/HTML)

#### form - [ko&#8677;]
Add the `.form--horizontal` class to have form labels to the left of the inputs:
```html
<form action="#"${1: class="form--horizontal"}>
	${2:<fieldset class="form-fieldset">
		<legend class="form-legend">Your form</legend>
		$3
	</fieldset>}
	$0
</form>
```

#### form item - [ko&#8677;]
```html
<div class="form-controlGroup">
	<label class="form-label" for="${1:name}">${2:Label}</label>
	<div class="form-controlGroup-inputWrapper">
		<input class="form-input" type="${3:text}" id="$1"${4: placeholder="Placeholder text"}/>
	</div>
</div>
```

#### form note - [ko&#8677;]
```html
<span class="form-note">?<span>First name &amp; last name</span></span>
```

#### Grid - Row - [ko&#8677;]
```html
<div class="g-row">

</div>
```

#### Grid - 2 columns - [ko&#8677;]
```html
<div class="g-row">
	<div class="g-span-6 g-col">

	</div>
	<div class="g-span-6 g-col">

	</div>
</div>
```

#### Grid - One column - [ko&#8677;]
```html
<div class="g-span-6 g-col">

</div>
```

#### Block grid - [ko&#8677;]
```html
<ul class="l-blockGrid l-blockGrid--${1:4up}${2: l-blockGrid--2up--narrow}">
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
	<li>Item 4</li>
</ul>
```

#### Button - primary - [ko&#8677;]
```html
<a href="${1:#}" class="btn btn--primary">${2:Button text}</a>
```

#### Button - [ko&#8677;]
```html
<a href="${1:#}" class="btn btn--primary">${2:Button text}</a>
```

#### Fluid video - [ko&#8677;]
```html
<div class="fluidVideo">
	${1:<iframe width="560" height="315" src="//www.youtube-nocookie.com/embed/-5Ae-LhMIG0" frameborder="0" allowfullscreen></iframe>}
</div>
```

#### Form actions - [ko&#8677;]
```html
<div class="form-actions text_centre">
	<input type="submit" value="Submit" class="btn btn--primary" />
	<input type="reset" class="btn" value="Cancel" />
</div>
```

#### Form - Custom checkboxes - [ko&#8677;]
```html
<!-- Custom checkboxes -->
<div class="form-controlGroup">
	<label class="form-label">Custom checkboxes</label>
	<div class="form-controlGroup-inputWrapper">
		<!-- Wrap checkbox elements with .control.control--custom.control--checkbox <label> -->
		<label class="control control--custom control--checkbox">
			<input type="checkbox" value="check4">
			<span class="control-indicator"></span>
			This is a custom checkbox
		</label>
		<label class="control control--custom control--checkbox">
			<input type="checkbox" value="check4">
			<span class="control-indicator"></span>
			This is a custom checkbox
		</label>
	</div>
</div>
```

#### Form - Custom radios - [ko&#8677;]
```html
<!-- Custom radio buttons -->
<div class="form-controlGroup g-span6 g-col">
	<label class="form-label">Radio buttons</label>
	<div class="form-controlGroup-inputWrapper">
		<!-- Wrap radio elements with .control.control--custom.control--radio <label> -->
		<label class="control control--custom control--radio">
			<input type="radio" name="optionsRadios" id="optionsRadios4" value="option4">
			<span class="control-indicator"></span>
			This is a custom radio button
		</label>
		<label class="control control--custom control--radio">
			<input type="radio" name="optionsRadios" id="optionsRadios4" value="option4">
			<span class="control-indicator"></span>
			This is a custom radio button
		</label>
	</div>
```

#### Form - inline radios - [ko&#8677;]
```html
<div class="form-controlGroup">
	<label class="form-label">Inline radio buttons</label>
	<div class="form-controlGroup-inputWrapper">
		<label class="control control--inline">
			<input type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked>
			This is a radio
		</label>
		<label class="control control--inline">
			<input type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
			This is another radio
		</label>
	</div>
</div>
```

#### Form - inline checkboxes - [ko&#8677;]
```html
<div class="form-controlGroup">
	<label class="form-label">Inline Checkboxes</label>
	<div class="form-controlGroup-inputWrapper">
		<label class="control control--inline">
			<input type="checkbox" value="check1">
			This is a checkbox
		</label>
		<label class="control control--inline">
			<input type="checkbox" value="check2">
			This is a checkbox
		</label>
	</div>
</div>
```

#### Form - checkbox - [ko&#8677;]
```html
<div class="form-controlGroup g-span6 g-col">
	<label class="form-label">Checkboxes</label>
	<div class="form-controlGroup-inputWrapper">
		<label class="control">
			<input type="checkbox" value="check1">
			This is a checkbox
		</label>
		<label class="control">
			<input type="checkbox" value="check2">
			This is a checkbox
		</label>
	</div>
</div>
```

#### Media object - [ko&#8677;]
```html
<div class="media">
	<div class="media-img${1: media--rev}">
		<img src="${2:/path/to/img.jpg}">
	</div>
	<div class="media-body">
		$3
	</div>
</div>
```

#### Table - [ko&#8677;]
```html
<table class="table${1: table--bordered}${2: table--striped}${3: table--hover}${4: table--rounded}" cellpadding="0" cellspacing="0">
	<thead>
		<th>Table head</th>
		<th>Table head</th>
		<th>Table head</th>
	</thead>
	<tbody>
		<tr>
			<td>Table cell</td>
			<td>Table cell</td>
			<td>Table cell</td>
		</tr>
	</tbody>
	<tfoot>
		<td>Table foot</td>
		<td>Table foot</td>
		<td>Table foot</td>
	</tfoot>
</table>
```

## CSS
[Reference](https://github.com/tmwagency/Kickoff-snippets/tree/master/CSS)

#### background - [ko&#8677;]
```css
background: ${1:#f2f2f2} url('/img/${2:/ui/}$3') ${4:left} ${5:top} ${6:no-repeat};$0
```

#### media-query - [ko&#8677;]
```css
/* === $1> === */
@media screen and (${2:min}-width: ${1:768px}) {
	$0
}
/* === end $1> === */
```

#### background-size - [ko&#8677;]
```css
background-size: ${1:cover};$0
/* === end 760> === */
```

#### border-radius - [ko&#8677;]
```css
border-radius: ${1:5px};$0
```

#### box-shadow - [ko&#8677;]
```css
box-shadow: ${1:0} ${2:1px} ${3:3px} ${4:rgba(0,0,0,.25)};$0
```

#### box-sizing - [ko&#8677;]
```css
box-sizing: ${1:border-box};
```

#### transition - [ko&#8677;]
```css
transition: ${1:all 200ms ease-in-out};
```

## Sass
[Reference](https://github.com/tmwagency/Kickoff-snippets/tree/master/SCSS)

#### font-size REM mixin - [ko&#8677;]
```
@include font-size(16);
```

#### line-height REM mixin - [ko&#8677;]
```
@include line-height(50);
```

#### linear-gradient - [ko&#8677;]
[Reference](https://github.com/tmwagency/kickoff/blob/master/scss/mixins/_linear-gradient.scss)
```
@include linear-gradient(left, #1e5799 0%, #2989d8 50%);
```

#### opacity - [ko&#8677;]
```
@include opacity(60);
```

#### respond-min - [ko&#8677;]
```
// === 760> ===
@include respond-min(760}) {
	[...]
}
// === end 760> ===
```

#### respond-max - [ko&#8677;]
```
// === 760> ===
@include respond-max(760}) {
	[...]
}
// === end 760> ===
```

#### respond-min-max - [ko&#8677;]
```
// === 100, 300 ===
@include respond-min-max(100, 300) {
	[...]
}
// === end 100, 300 ===
```

#### size (sizing an element - w x h) - [ko&#8677;]
```
@include size(10px,10px);
```

#### square (for elements with same height & width) - [ko&#8677;]
```
@include square(50px);
```

#### transition - [ko&#8677;]
```
@include transition(all 200ms ease-in-out);
```

## Javascript
[Reference](https://github.com/tmwagency/Kickoff-snippets/tree/master/Javascript)

#### object - [ko&#8677;]
```js
KO.? = {
	init : function() {
		var that = this;

	}
};
```
