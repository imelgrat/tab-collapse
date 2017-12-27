# Tab/Collapse
While Bootstrap's Collapse component (accordions) can be very useful and works well in mobile websites, tab-based navigation usually works better in desktop screens. This component provides a way to integrate both tabs and accordions using some extra CSS and Javascript.

Developed by [Ivan Melgrati](https://imelgrat.me) [![Twitter](https://img.shields.io/twitter/url/https/github.com/imelgrat/tab-collapse.svg?style=social)](https://twitter.com/imelgrat)

License: [![GitHub license](https://img.shields.io/github/license/imelgrat/tab-collapse.svg)](https://github.com/imelgrat/tab-collapse/blob/master/LICENSE)

Status: [![GitHub release](https://img.shields.io/github/release/imelgrat/tab-collapse.svg)](https://github.com/imelgrat/tab-collapse) [![GitHub issues](https://img.shields.io/github/issues/imelgrat/tab-collapse.svg)](https://github.com/imelgrat/tab-collapse/issues) [![GitHub forks](https://img.shields.io/github/forks/imelgrat/tab-collapse.svg)](https://github.com/imelgrat/tab-collapse/network) [![GitHub stars](https://img.shields.io/github/stars/imelgrat/tab-collapse.svg)](https://github.com/imelgrat/tab-collapse/stargazers)


Requirements
------------

*   jQuery >= 3.0
*   Bootstrap >= 3.3

Installation
------------

While most of the code required to make tabs and accordions work comes from Bootstrap, it is necessary to add some extra code to make the "component switch" between tabs and accordions view and navigation work.
After adding both jQuery and Bootstrap, it's necessary to add the component's CSS rules and JavaScript code

```html
<link rel="stylesheet" href="../dist/css/tabcollapse-style.css" crossorigin="anonymous">
<script src="../dist/js/tabcollapse-script.js" crossorigin="anonymous"></script>
```

Usage
------------
For the Tab/Collapse to work, it's necessary to create three blocks. The *vertab-container* div (the whole component's container, used as CSS and JS selector), the *vertab-menu* section (tab navigation links) and the *vertab-accordion* section (accordion and content sections). 
For each content section, it's necessary to create a link inside the *list-group* block and a *vertab-content* block.

```html
<div class="col-lg-12 vertab-container">
	<div class="col-lg-3 col-md-3 col-sm-3 vertab-menu">
		<div class="list-group">
			<a href="#" class="list-group-item text-left"> This is Tab 1 </a>
			.......
		</div>
	</div>
	<div id="accordion" class="col-lg-9 col-md-9 col-sm-9 col-xs-12 vertab-accordion panel-group">
		<div class="vertab-content">
			<div class="panel-heading">
				<h4 class="panel-title" data-toggle="collapse" data-parent="#accordion" data-target="#collapse1"> This is Heading 1 </h4>
			</div>
			<div id="collapse1" class="panel-collapse collapse">
				<div class="panel-body">
					Here goes the content
				</div>
			</div>
		</div>
		......... 
	</div>
</div>
```
Feedback
--------

Please open an issue to request a feature or submit a bug report. Or even if
you just want to provide some feedback, I'd love to hear. I'm also available on
Twitter as [@imelgrat](https://twitter.com/imelgrat).

Contributing
------------

1.  Fork it.
2.  Create your feature branch (`git checkout -b my-new-feature`).
3.  Commit your changes (`git commit -am 'Added some feature'`).
4.  Push to the branch (`git push origin my-new-feature`).
5.  Create a new Pull Request.

Links
====
* Article/Tutorial: https://imelgrat.me/javascript/integrate-bootstrap-tabs-accordions/
* Live example: https://codepen.io/imelgrat/details/wpGgpN/
