# photo-gallery
Graphics have taken on an increasingly central role to online content and the need for interactive and beautifully designed photo galleries has never been more prevalent. In this article we will show you how to build a photo gallery for your website either using pure HTML, CSS, and JavaScript or by using the Solodev Templating Language.

## Tutorial

For detailed instructions, view Solodev's [How to Build a Photo Gallery Four Your Website](https://www.solodev.com/blog/web-design/code-examples/how-to-build-a-photo-gallery-for-your-website.stml) article.

## Demo

Check out a working example on [JSFiddle](https://jsfiddle.net/solodev/kmk2abtf/).

## HTML

The photo gallery includes basic HTML markup for displaying images.
```
<div id="imagesContainer">
<div title="images" id="images">
<div class="row">
<div class="col-md-3">
   <div class="fg-listItem">
      <div style="overflow: hidden; border-color: rgb(189, 195, 199); padding: 3px; background-color: rgb(245, 245, 245);">
         <div class="fg-thumbnail-container" style="height: 190px; overflow: hidden;">
            <img class="fg-thumb" src="https://www.solodev.com/assets/fancy/travel2.jpg" alt="" style="display: block; max-width: none; height: 190px; opacity: 1;">
         </div>
         <div class="fg-title fg-title-outside" style="color: rgb(44, 62, 80); width: 100%; display: none; background: rgb(245, 245, 245);">
         </div>
      </div>
      <img src="https://www.solodev.com/assets/fancy/shadow.png" class="fg-shadow">
   </div>
</div>
<div class="col-md-3">
   <div class="fg-listItem">
      <div style="overflow: hidden; border-color: rgb(189, 195, 199); padding: 3px; background-color: rgb(245, 245, 245);">
         <div class="fg-thumbnail-container" style="height: 190px; overflow: hidden;">
            <img class="fg-thumb" src="https://www.solodev.com/assets/fancy/travel3.jpg" alt="" style="display: block; max-width: none; height: 190px; opacity: 1;">
         </div>
         <div class="fg-title fg-title-outside" style="color: rgb(44, 62, 80); width: 100%; display: none; background: rgb(245, 245, 245);">
         </div>
      </div>
      <img src="https://www.solodev.com/assets/fancy/shadow.png" class="fg-shadow">
   </div>
</div>
<div class="col-md-3">
   <div class="fg-listItem">
      <div style="overflow: hidden; border-color: rgb(189, 195, 199); padding: 3px; background-color: rgb(245, 245, 245);">
         <div class="fg-thumbnail-container" style="height: 190px; overflow: hidden;">
            <img class="fg-thumb" src="https://www.solodev.com/assets/fancy/travel4.jpg" alt="" style="display: block; max-width: none; height: 190px; opacity: 1;">
         </div>
         <div class="fg-title fg-title-outside" style="color: rgb(44, 62, 80); width: 100%; display: none; background: rgb(245, 245, 245);">
         </div>
      </div>
      <img src="https://www.solodev.com/assets/fancy/shadow.png" class="fg-shadow">
   </div>
</div>
<div class="col-md-3">
   <div class="fg-listItem">
      <div style="overflow: hidden; border-color: rgb(189, 195, 199); padding: 3px; background-color: rgb(245, 245, 245);">
         <div class="fg-thumbnail-container" style="height: 190px; overflow: hidden;">
            <img class="fg-thumb" src="https://www.solodev.com/assets/fancy/travel5.jpg" alt="" style="display: block; max-width: none; height: 190px; opacity: 1;">
         </div>
         <div class="fg-title fg-title-outside" style="color: rgb(44, 62, 80); width: 100%; display: none; background: rgb(245, 245, 245);">
         </div>
      </div>
      <img src="https://www.solodev.com/assets/fancy/shadow.png" class="fg-shadow">
   </div>
</div>
</div>
```
# CSS

All necessary CSS is in photo-gallery.css

## JavaScript

JavaScript (jQuery) to add effects to the photo gallery is stored in photo-gallery.js
```
$('#imagesContainer').fancygallery({
   navigation: 'pagination', 
   titleHoverEffect: 'none', 
   rowOffset: 25, 
   thumbWidth: 250, 
   thumbHeight: 190, 
   lightbox: 'fancybox'
   });
```
## External Includes
```
<link rel="stylesheet" href="https://www.solodev.com/assets/fancy/jquery-fancygallery.css">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link rel="stylesheet" href="photo-gallery.css">

<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.4/jquery.min.js"></script>
<script type="text/javascript" src="https://www.solodev.com/assets/fancy/jquery-fancygallery.js"></script>
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/fancybox/2.1.5/jquery.fancybox.pack.js"></script>
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/fancybox/2.1.5/jquery.fancybox.js"></script>
<script type="text/javascript" src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script type="text/javascript" src="photo-gallery.js."></script>
```
