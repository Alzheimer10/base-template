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