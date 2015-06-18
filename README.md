# Supa Simple Grid
Pretty much just a clone of Chris Nager's amazing [Ungrid](http://chrisnager.github.io/ungrid) with a bit of extra flair.

## Installation
Copy and paste the contents of grid.css into your css file.

## Usage
To use, simply put as many .cols as you wish in your .rows and the .cols will automatically be evenly spaced.

```html
<div class="row">
	<div class="col">Col</div>
	<div class="col">Col</div>
	<div class="col">Col</div>
	...
	<div class="col">Col</div>
</div>
```

Want gutters? Add a .grid wrapper around your rows.
```html
<div class="grid">
	<div class="row">
		<div class="col">Col</div>
		<div class="col">Col</div>
		<div class="col">Col</div>
		...
		<div class="col">Col</div>
	</div>
</div>
```

Want custom column widths? Create some classes or set the width inline.
```css
.col-1-2 { width: 50%; }
.col-1-3 { width: 33.333333%; }
.col-2-3 { width: 66.666666%; }
.col-1-4 { width: 25%; }
.col-3-4 { width: 75%; }
```

```html
<h2>Custom Column Widths</h2>
<div class="grid">
	<div class="row">
		<div class="col col-1-3">col-1-3</div>
		<div class="col col-2-3">col-2-3</div>
	</div>
	<div class="row">
		<div class="col col-1-4">col-1-4</div>
		<div class="col col-1-2">col-1-2</div>
		<div class="col col-1-4">col-1-4</div>
	</div>
	<div class="row">
		<div class="col" style="width:10%;">10%</div>
		<div class="col" style="width:20%;">20%</div>
		<div class="col" style="width:30%;">30%</div>
		<div class="col" style="width:40%;">40%</div>
	</div>
</div>
```

Nested columns? Sure, it's like a throwback to nested tables.
```html
<div class="row">
	<div class="col">
		Outer Col
		<div class="row">
			<div class="col">Nested Col</div>
			<div class="col">Nested Col</div>
		</div>
	</div>
	<div class="col">Outer Col</div>
</div>
```


##License
The MIT License (MIT)

Copyright (c) 2015 Michael Gillihan

Ungrid - Copyright (c) 2014-2015 Chris Nager

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.