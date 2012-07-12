# Kickoff Snippets for Sublime Text 2

Use these snippets if you use my Boost framework & Sublime Text

* Example page https://github.com/tmwagency/kickoff/blob/master/index.html
* Grids: http://mrmartineau.github.com/Choreographic-Grid/test.html

## Tab trigger for all items: 'ko:' &#8677;

## Forms

### form - ko:&#8677;

Remove the 'form_stacked' class to have form labels to the left of the inputs

```html
<form action="#" class="form-horizontal">
	<fieldset>
		<legend>Your form</legend>

	</fieldset>
</form>
```

### form items - ko:&#8677;

```html
<ul class="control-group">
	<li class="control-item">
		<label for="name" class="control-label">Name</label>
		<div class="control-input">
			<input type="text" id="name" placeholder="Zander Martineau" />
		</div>
	</li>
	<li class="control-item">
		<label for="email" class="control-label">Email</label>
		<div class="control-input">
			<input type="email" id="email" placeholder="zmartineau@tmw.co.uk" />
		</div>
	</li>
	<li class="control-item">
		<label for="phone" class="control-label">Phone</label>
		<div class="control-input">
			<input type="number" id="phone" placeholder="020 123 4567" />
		</div>
	</li>
	<li class="control-item">
		<label for="comments" class="control-label">Comments</label>
		<div class="control-input">
			<textarea id="comments" rows="3" cols="50" class="input-xlarge"></textarea>
		</div>
	</li>
</ul>
```

### form item - ko:&#8677;

```html
<li class="control-item">
	<label for="name" class="control-label">Name</label>
	<div class="control-input">
		<input type="text" id="name" placeholder="Zander Martineau" />
	</div>
</li>
```

### form note - ko:&#8677;

```html
<span class="form-note">?<span>First name &amp; last name</span></span>
```

## Grid

### Row - ko:&#8677;

```html
<div class="row">

</div>
```

### 2 columns - ko:&#8677;

```html
<div class="row">
	<div class="span-6 col">

	</div>
	<div class="span-6 col">

	</div>
</div>
```

### One column - ko:&#8677;

```html
<div class="span-6 col">

</div>
```

## LESS mixins
These reference https://github.com/mrmartineau/Boost/blob/master/less/mixins.less

### border-radius - ko:&#8677;

```
.border-radius(5px);
```

### box-shadow - ko:&#8677;

```
.box-shadow(0 1px 3px rgba(0,0,0,.25));
```

### opacity - ko:&#8677;

```
.opacity(60);
```

### size (sizing an element - w x h) - ko:&#8677;

```
.size(10px,10px);
```

### square (for elements with same height & width) - ko:&#8677;

```
.square(50px);
```

### font-size REM mixin - ko:&#8677;

```
.font-size(16);
```

### line-height REM mixin - ko:&#8677;

```
.line-height(50px);
```