# Boost Snippets for Sublime Text 2

Use these snippets if you use my Boost framework & Sublime Text

* Example page http://mrmartineau.github.com/Boost/example.html
* Grids: http://mrmartineau.github.com/Boost/grid.html

## Forms
Tab triggers are listed by the titles

### form - bform&#8677;

Remove the 'form_stacked' class to have form labels to the left of the inputs

```
<form action="#" class="form_stacked">

</form>
```

### form li - bformitem&#8677;

```
<li>
	<label for="name">Label</label>
	<div class="input">
		<input type="text" id="name" placeholder="Zander Martineau" />
	</div>
</li>
```

### form ul - bformitems&#8677;

```
<ul>
	<li>
		<label for="name">Name</label>
		<div class="input">
			<input type="text" id="name" placeholder="Zander Martineau" />
		</div>
	</li>
	<li>
		<label for="email">Email</label>
		<div class="input"><input type="email" id="email" placeholder="zander@martineau.tv" /></div>
	</li>
	<li>
		<label for="phone">Phone</label>
		<div class="input"><input type="number" id="phone" placeholder="020 123 4567" /></div>
	</li>
	<li>
		<label for="comments">Comments</label>
		<div class="input">
			<textarea id="comments" rows="3" cols="50"></textarea>
		</div>
	</li>
</ul>
```

### form note - bformnote&#8677;

```
<span class="form_note">?<span>First name &amp; last name</span></span>
```

## Grid

### Row - brow&#8677;

```
<div class="row">

</div>
```

### 2 columns - b2col&#8677;

```
<div class="row">
	<div class="grid_6 column">

	</div>
	<div class="grid_6 column">

	</div>
</div>
```

### One column - bcol&#8677;

```
<div class="grid_6 column">

</div>
```

## LESS mixins
These reference https://github.com/mrmartineau/Boost/blob/master/less/mixins.less

### border-radius - bbr&#8677;

```
.border-radius(5px);
```

### box-shadow - bbs&#8677;

```
.box-shadow(0 1px 3px rgba(0,0,0,.25));
```

### opacity - .opacity(60)&#8677;

```
.opacity(60);
```

### size (sizing an element - w x h)- bs&#8677;

```
.size(10px,10px);
```

### square (for elements with same height & width) - bsq&#8677;

```
.square(50px);
```