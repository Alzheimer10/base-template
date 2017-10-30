<p align="center">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/BOOTSTRAP.png?raw=true" width="10%">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/HTML.png?raw=true" width="10%">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/CSS3.png?raw=true" width="10%">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/JS.png?raw=true" width="10%">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/SASS.png?raw=true" width="10%">
<img src="https://github.com/Alzheimer10/base-template/blob/master/img/icon-vendor/JQUERY.png?raw=true" width="10%">
</p>

# TEMPLATE HTML-5 - BOOTSTRAP-3
Base Template V0.0.1
Author: Carlos Anselmi carlosanselmi2@gmail.com

### VENDORS
* `Bootstrap`		-	framework-front-end 3.7
* `jquery`			-	jquery
* `Font-Awesome`	-	fonts-icons
* `animatescroll`	-	animation scroll
* `scrollreveal`	-	animation css
* `prefixfree`		-	Prefijos navegadores css
* `FullPage`		-	FullPage

### GOTOTOP
**HTML**
```html
<!-- botton-gotop -->
<div class="ac-gototop gototop-square" onclick="$('body').animatescroll({scrollSpeed:1000});">
	<a class="js-gotop"><i class="fa fa-chevron-up fa-x2" aria-hidden="true"></i></a>
</div>
<!-- END-BOTTON-GOTOP -->
```
**JAVASCRIPT**
```javascript
var loaderPage = function() {
	$(window).load(function(){
		$('body').removeClass('ac-scroll-loader');
		$(".ac-loader").fadeOut("slow");
	});
},
```

### FullPage
**HTML**
```html
<div id="fullpage">
	<div class="section text-center">
		<h1>Some section 1</h1>
	</div>
	<div class="section" id="section02" >
		<div class="slide text-center">
			<h1>Some section 3</h1>
		</div>
		<div class="slide text-center active">
			<div>	
				<h1>SLIDE 1</h1>
			</div>
			<div>
				<h1>SLIDE 2</h1>						
			</div>
		</div>
		<div class="slide text-center">
			<h1>SLIDE 3</h1>
		</div>
	</div>
	<div class="section">Some section 2</div>
	<div class="section">Some section 3</div>
</div>
```

**JAVASCRIPT**
```javascript
	$(document).ready(function() {
		$('#fullpage').fullpage({
			//Navigation
			menu: '#menu',
			lockAnchors: false,
			anchors:['firstPage', 'secondPage'],
			navigation: true,
			navigationPosition: 'right',
			navigationTooltips: [],
			showActiveTooltip: false,
			slidesNavigation: true,
			slidesNavPosition: 'bottom',

			//Scrolling
			css3: true,
			scrollingSpeed: 700,
			autoScrolling: true,
			fitToSection: true,
			fitToSectionDelay: 1000,
			scrollBar: true,
			easing: 'easeInOutCubic',
			easingcss3: 'ease',
			loopBottom: false,
			loopTop: false,
			loopHorizontal: false,
			continuousVertical: false,
			continuousHorizontal: false,
			scrollHorizontally: false,
			interlockedSlides: false,
			dragAndMove: false,
			offsetSections: false,
			resetSliders: false,
			fadingEffect: false,
			normalScrollElements: '#element1, .element2',
			scrollOverflow: false,
			scrollOverflowReset: false,
			scrollOverflowOptions: null,
			touchSensitivity: 15,
			normalScrollElementTouchThreshold: 5,
			bigSectionsDestination: null,

			//Accessibility
			keyboardScrolling: true,
			animateAnchor: true,
			recordHistory: true,

			//Design
			controlArrows: true,
			verticalCentered: true,
			sectionsColor : ['black', 'red' , 'blue'],
			paddingTop: '3em',
			paddingBottom: '10px',
			fixedElements: '#header, .footer',
			responsiveWidth: 0,
			responsiveHeight: 0,
			responsiveSlides: false,
			parallax: true,
			parallaxOptions: {type: 'reveal', percentage: 62, property: 'translate'},

			//Custom selectors
			sectionSelector: '.section',
			slideSelector: '.slide',

			lazyLoading: true,

			//events
			onLeave: function(index, nextIndex, direction){},
			afterLoad: function(anchorLink, index){},
			afterRender: function(){},
			afterResize: function(){},
			afterResponsive: function(isResponsive){},
			afterSlideLoad: function(anchorLink, index, slideAnchor, slideIndex){},
			onSlideLeave: function(anchorLink, index, slideIndex, direction, nextSlideIndex){}
		});
	});
```