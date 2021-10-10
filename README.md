# Simple and media spoilers

## Description

Responsive regular and screen size dependent spoilers using javascript

## Examples 👁️

![screenshot](https://user-images.githubusercontent.com/91592743/136660487-62c240d5-dcbc-4ce6-9aa9-a62859f68a79.png)

https://user-images.githubusercontent.com/91592743/136660482-4919a181-8a5f-4685-b691-acf35f7a5283.mp4

---

## Technologies used 🛠️

<h3 align="left"> &nbsp  &nbsp  &nbsp Programming languages</h3>

<a href="https://www.w3.org/html/" target="_blank"> <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" height="30"/> </a>
<a href="https://www.w3schools.com/css/" target="_blank"> <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" height="30"/> </a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript" height="30"/> </a>

---

## Features 💡

⚡️ Regular and media query dependent spoilers\
⚡️ Accordion spoilers\
⚡️ Easy to use\
⚡️ Customizable

## How To Use 🔧

For the spoiler parent, write the `data-spoilers` attribute. For the slider headers, write the `data-spoiler` attribute

If you need to turn on / off the spoilers on different screen sizes, write the parameters of the width and type of breakpoint.

For example:

- `data-spoilers = "992, max"` spoilers will only work on screens less than or equal to 992px
- `data-spoilers - "768, min"` spoilers will only work on screens greater than or equal to 768px

If you need only one spoiler (accordion) to be opened in the block, add the `data-one-spoiler` attribute

If you need the spoiler to be open when the site is loaded (by default), you need to add the `_active` class for the spoiler titles (.block\_\_title)

Examples:

Regular accordion spoiler:

```html
<div data-spoilers data-one-spoiler class="block block_1">
	<div class="block__item">
		<button tabindex="-1" type="button" data-spoiler class="block__title">
			Simple spoiler #1
		</button>

		<div class="block__text">Lorem ipsum dolor sit amet!</div>
	</div>

	<div class="block__item">
		<button
			tabindex="-1"
			type="button"
			data-spoiler
			class="block__title _active"
		>
			Simple spoiler #2
		</button>
		<div class="block__text">Lorem ipsum dolor sit amet!</div>
	</div>
</div>
```

Screen size dependent spoiler (width >= 650px):

```html
<div data-spoilers="650,min" class="block block_2">
	<div class="block__item">
		<button tabindex="-1" type="button" data-spoiler class="block__title">
			This spoiler works on screen width >= 650px
		</button>
		<div class="block__text">Lorem ipsum dolor sit amet!</div>
	</div>
</div>
```

Screen size dependent spoiler (width <= 800px):

```html
<div data-spoilers="800,max" class="block block_3">
	<div class="block__item">
		<button tabindex="-1" type="button" data-spoiler class="block__title">
			#1 Spoiler works on screen width <= 800px
		</button>
		<div class="block__text">Lorem ipsum dolor sit amet!</div>
	</div>
</div>
```

---

## Acknowledgments 🎁

Thanks to
[Евгений Андриканич](https://fls.guru/) ,
[Vladilen Minin](https://www.youtube.com/c/VladilenMinin) ,
[CS50](https://cs50.harvard.edu/college/2021/fall/) ,
[Александр Лущенко](https://itgid.info/) ,
[Vadim Makeev](https://www.youtube.com/channel/UCaTfYudJUVA8cV_But8KZVQ) ,
[Safak](https://github.com/safak) ,
[Adrian Hajdin](https://www.completepathtojavascriptmastery.com/) ,
[Sumit Dey](https://www.youtube.com/c/BackbenchCoder)
for motivational and helpful content

---
