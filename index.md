---
layout: default
title: Capability Wise Pty Ltd- Home
---


<div class="content-zone-1">
<div class="content-block-1">

<h1>Digital Transformation..</h1>

..is more that just creating new websites and APIs.  Digital transformation is about reimagining the way you delivery services to your customers and establishing the right capabilities to consistently exceed their expectations.

<br/>
Digital transformation should turn you current business processes on their head and ensure that you are delighting your customers.
<br/>
<b>Anything short of that is just digitisation.</b>
<br/><br/>
</div>
</div>

<div class="content-zone-2">
<div class="content-block-1">
<h2>News and Events</h2>

<div>
<style>
.mySlides {display:none}
.w3-left, .w3-right, .w3-badge {cursor:pointer}
.w3-left{float:left!important}
.w3-right{float:right!important}
.w3-badge {background-color:#000;color:#fff;display:inline-block;padding:0px;text-align:center;height:13px;width:13px; border-radius:50%}
.w3-border{border:1px solid #ccc!important}
.w3-padding-left{padding-left:16px!important}.w3-padding-right{padding-right:16px!important}
.w3-transparent{background-color:transparent!important}
.w3-white,.w3-hover-white:hover{color:#000!important;background-color:#fff!important}
.w3-hover-text-khaki:hover{color:#b4aa50!important}
.w3-display-bottommiddle{
position:absolute;
bottom:0;
opacity:0.7;
width:100%;
text-align:center
}
.w3-center{display:inline-block}
.w3-large{font-size:18px!important}
.w3-section{margin-top:16px!important}
.w3-content{max-width:980px;margin:auto;font-family:Verdana,sans-serif;font-size:15px;line-height:1.5;overflow-x:hidden}
.w3-container{padding:0.01em 16px}
.w3-container:after,.w3-container:before{content:"";display:table;clear:both}
.w3-display-container{position:relative;border:solid;}
</style>

<div class="w3-content w3-display-container" style="max-width:800px;max-height:600px">
<div class="mySlides" style="text-align:center;">
<table>
<tr>
<td>
<a href="https://goo.gl/TaS2Ba"><img src="{{site.url | absolute}}/images/SydneySummit.jpg"/></a>
</td>
<td>
<img src="{{site.url | absolute}}/images/ml-photo.jpg" width="200px"/><br/>
Our Managing Director, Matt Lewis will be presenting at the WSO2 Sydney Summit 2017.  
<br/><br/><a href="https://goo.gl/TaS2Ba">Book your tickets today.</a>
</td>
</tr>
</table>
</div>

<div class="mySlides" style="text-align:center;">
<table>
<tr>
<td>
The Digital Business Council has released the Interoperabilty Framework for eInvoicing.
</td>
</tr>
</table>
/div>

  <div class="w3-center w3-section w3-large w3-text-white w3-display-bottommiddle" >
    <span class="w3-badge dotObjects w3-border w3-transparent w3-hover-white" onclick="currentDiv(1)"></span>
    <span class="w3-badge dotObjects w3-border w3-transparent w3-hover-white" onclick="currentDiv(2)"></span>
  </div>
</div>
  
<script>
var slideIndex = 1;
showDivs(slideIndex);

function plusDivs(n) {
  showDivs(slideIndex += n);
}

function currentDiv(n) {
  showDivs(slideIndex = n);
}

function showDivs(n) {
  var i;
  var x = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dotObjects");
  if (n > x.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = x.length}
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
     dots[i].className = dots[i].className.replace(" w3-white", "");
  }
  x[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " w3-white";
}
</script>

</div>
<br>
</div>

</div>

<div class="content-zone-3">
<div class="content-block-1">
<h2>Our Services</h2>

<table>
<tr>
<td><img src="{{site.url | absolute}}/images/product-2.png"/></td>
<td><b>Consulting Services</b><br/>
Capability Wise can assist with all your digital transformation needs.  We provide consulting services across the full transformation lifecycle from helping you establish a clear vision, through to execution of your transformation strategy, and ultimately establishment of the appropriate capabilities to sustain your market advantage.
<br/>
Our key consulting services include:
<ul>
<li>Digital Strategy and Execution</li>
<li>Digital Transformation Planning</li>
<li>Enterprise Agility</li>
<li>Standards Adoption and Cross-Industry Interoperability</li>
<li>Business Process Reinvention</li>
</ul>

<b>Find Out More --></b>
</td>
</tr>
<tr>

<td><img src="{{site.url | absolute}}/images/product-3.png"/></td>
<td>Technology Services
<br/>
Unlike other technology services companies we are not all things to all customers.  We have specialised on two niche offerings that enable us to provide leading edge solutions to our customers at the best possible price point.  OUr tow specialties are:
<ul>
<li>Blockchain; and </li>
<li>APIs and Microservices.</li>
</ul>

</td>

</tr>
</table>

</div>
</div>
