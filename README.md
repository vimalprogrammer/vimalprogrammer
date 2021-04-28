<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:version='2' class='v2' expr:dir='data:blog.languageDirection' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <meta content='ldK_O2Pchwj_z3CQ0Zwr2AmYbebkPhZx05N99Hw0T80' name='google-site-verification'/>
    <meta content='width=device-width, initial-scale=1, maximum-scale=1' name='viewport'/>
<script src='https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js' type='text/javascript'/>   
<link href='http://fonts.googleapis.com/css?family=Open+Sans:400,400i,600,600i,700,700i|Indie+Flower' media='all' rel='stylesheet' type='text/css'/>
    <link href='//maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css' rel='stylesheet'/>
 <link href='//cdn.linearicons.com/free/1.0.0/icon-font.min.css' rel='stylesheet'/>

    <b:include data='blog' name='all-head-content'/>
    <title>
		<b:if cond='data:blog.pageType == &quot;index&quot;'>
			<data:blog.pageTitle/>
		<b:else/>
			<b:if cond='data:blog.pageType != &quot;error_page&quot;'>
				<data:blog.pageName/> - <data:blog.title/>
			<b:else/>
				ERROR 404 - <data:blog.title/> 
			</b:if>
		</b:if>
    </title>
    <!-- Description and Keywords (start) -->
    <b:if cond='data:blog.pageType == &quot;index&quot;'>
    <meta content='YOUR DESCRIPTION HERE' name='description'/>
    </b:if>
    <meta content='YOUR KEYWORDS HERE' name='keywords'/>
    <!-- Description and Keywords (end) -->
    <b:if cond='data:blog.pageType == &quot;item&quot;'>
        <meta expr:content='data:blog.pageName' property='og:title'/>
        <meta expr:content='data:blog.canonicalUrl' property='og:url'/>
        <meta content='article' property='og:type'/>
    </b:if>
    <b:if cond='data:blog.postImageUrl'>
        <meta expr:content='data:blog.postImageUrl' property='og:image'/>
    <b:else/>
    <b:if cond='data:blog.postImageThumbnailUrl'>
        <meta expr:content='data:blog.postImageThumbnailUrl' property='og:image'/>
    </b:if></b:if>
    <b:if cond='data:blog.metaDescription != &quot;&quot;'>
        <meta expr:content='data:blog.metaDescription' name='og:description'/>
    </b:if>
    <meta expr:content='data:blog.title' property='og:site_name'/>
    <meta expr:content='data:blog.homepageUrl' name='twitter:domain'/>
    <meta expr:content='data:blog.pageName' name='twitter:title'/>
    <b:if cond='data:blog.postImageUrl'>
      <meta content='summary_large_image' name='twitter:card'/>
      <meta expr:content='data:blog.postImageUrl' name='twitter:image'/>
    <b:else/>
      <meta content='summary' name='twitter:card'/>
      <b:if cond='data:blog.postImageThumbnailUrl'>
        <meta expr:content='data:blog.postImageThumbnailUrl' name='twitter:image'/> 
      </b:if>
    </b:if>
    <meta expr:content='data:blog.pageName' name='twitter:title'/>
    <b:if cond='data:blog.metaDescription'>
      <meta expr:content='data:blog.metaDescription' name='twitter:description'/>
    </b:if>
    <!-- Social Media meta tag need customer customization -->
    <meta content='Facebook App ID here' property='fb:app_id'/> 
    <meta content='Facebook Admin ID here' property='fb:admins'/> 
    <meta content='@username' name='twitter:site'/>
    <meta content='@username' name='twitter:creator'/>   
  <b:skin><![CDATA[/* 
-----------------------------------------------
Blogger Template Style
Name:        Vimal's Blog! :)
Author :     https://vimalprogrammer.blogspot.com/
License:     Free Version
----------------------------------------------- */
/* Variable definitions
-----------------------
<Group description="Main Hover Color" selector="body">
<Variable name="maincolor" description="Primary Color" type="color" default="#1976D2"  value="#1976D2"/>
</Group>
<Group description="Footer Color" selector="body">
<Variable name="footercolor" description="Bottom Footer Color" type="color" default="#1976D2"  value="#1976D2"/>
</Group>
/*****************************************
reset.css
******************************************/
html, body, .section, .widget, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, font, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td, figure {    margin: 0;    padding: 0;}
html {   overflow-x: hidden;}
a {text-decoration:none;color:#000;}
article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section {     display:block;}
table {    border-collapse: separate;    border-spacing: 0;}
caption, th, td {    text-align: left;    font-weight: normal;}
blockquote:before, blockquote:after,
q:before, q:after {    content: "";}
.quickedit, .home-link{display:none;}
blockquote, q {    quotes: "" "";}
sup{    vertical-align: super;    font-size:smaller;}
code{    font-family: 'Courier New', Courier, monospace;    font-size:12px;    color:#272727;}
::selection {background:transparent; text-shadow:#000 0 0 2px;}
::-moz-selection {background:transparent; text-shadow:#000 0 0 2px;}
::-webkit-selection {background:transparent; text-shadow:#000 0 0 2px;}
::-o-selection {background:transparent; text-shadow:#000 0 0 2px;}
a img{	border: none;}
ol, ul { padding:0;  margin:0;  text-align: left;  }
ol li { list-style-type: decimal;  padding:0 0 5px;  }
ul li { list-style-type: disc;  padding: 0 0 5px;  }
ul ul, ol ol { padding: 0; }
#navbar-iframe, .navbar {   height:0px;   visibility:hidden;   display:none   }
.Attribution, .feed-links, .post-footer-line.post-footer-line-1, .post-footer-line.post-footer-line-2 , .post-footer-line.post-footer-line-3 {
display: none;
}
.item-control {
display: none !important;
}
h2.date-header, h4.date-header {display:none;margin:1.5em 0 .5em}
h1, h2, h3, h4, h5, h6 {
    font-weight: 400;
    color: #151515;
}
img {
max-width: 100%;
vertical-align: middle;
border: 0;
}
*, *:before, *:after {
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
}
.widget iframe, .widget img {
max-width: 100%;
}
.status-msg-wrap {
display: none;
}
#preloader {
    position: fixed;
    z-index: 1800;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
   background-color: #242F3F;
}
.no-js #preloader,
.oldie #preloader {
    display: none
}
#loader {
    position: absolute;
    top: calc(50% - 1.25em);
    left: calc(50% - 1.25em);
}
.loader {
  display: inline-block;
  width: 30px;
  height: 30px;
  position: relative;
  border: 4px solid #Fff;
  top: 50%;
  animation: loader 2s infinite ease;
}

.loader-inner {
  vertical-align: top;
  display: inline-block;
  width: 100%;
  background-color: #fff;
  animation: loader-inner 2s infinite ease-in;
}

@keyframes loader {
  0% {
    transform: rotate(0deg);
  }
  
  25% {
    transform: rotate(180deg);
  }
  
  50% {
    transform: rotate(180deg);
  }
  
  75% {
    transform: rotate(360deg);
  }
  
  100% {
    transform: rotate(360deg);
  }
}

@keyframes loader-inner {
  0% {
    height: 0%;
  }
  
  25% {
    height: 0%;
  }
  
  50% {
    height: 100%;
  }
  
  75% {
    height: 100%;
  }
  
  100% {
    height: 0%;
  }
}
/*****************************************
Custom css starts
******************************************/
body {
color: #2e2e2e;
    font-family:"Open Sans", sans-serif;
font-size: 14px;
font-weight: normal;
line-height: 21px;
background: #f5f5f5;
}
/* ######## Wrapper Css ######################### */
#outer-wrapper{max-width:100%;margin:0 auto;background-color:#f5f5f5;box-shadow:0 0 5px RGBA(0, 0, 0, 0.2)}
.row{width:1170px}
#content-wrapper {
margin: 0 auto;
padding: 20px 0 30px;
}
.index #content-wrapper, .archive #content-wrapper {
overflow: hidden;
}
.item #main-wrapper, .statc_page #main-wrapper {
float: left;
width: 68%;
max-width: 800px;
}
.index #main-wrapper, .archive #main-wrapper {
float:none;
width:100%;
max-width:100%
}
.item #sidebar-wrapper, .statc_page #sidebar-wrapper {
float: right;
width: 30%;
max-width: 330px;
}
.index #sidebar-wrapper, .archive #sidebar-wrapper {
display:none;
visibility:hidden;
height:0;
opacity:0;
}
/* ######## Scrolling Navigation Menu Css ######################### */
.scroll-header {
       z-index: 9;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 10px 0px;
transition: all .5s;
display:none;
}
.item .scroll-header, .static_page .scroll-header, .error_page .scroll-header {
    position: static;
    display: flex;
    background: #fff none repeat scroll top left;
    box-shadow: 0 0 6px 1px rgba(0,0,0,0.1);
    padding: 20px 0;
}
.scroll-head-wrap {
margin:0 auto;
}
.item .scroll-header h1, .static_page .scroll-header h1, .error_page .scroll-header h1 {
color:#000!important;
}
.item .scroll-header #header img, .static_page .scroll-header #header img, .error_page .scroll-header #header img {
    display: block!important;
}
.item .scroll-header.scrolled-header h1, .static_page .scroll-header.scrolled-header h1, .error_page .scroll-header.scrolled-header h1 {
    display: none!important;
color:#000!important;
}
.item .scroll-header.scrolled-header #header img, .static_page .scroll-header.scrolled-header #header img, .error_page .scroll-header.scrolled-header #header img {
    display: block!important;
}
.scrollin-logo {
    float: left;
    margin: 0;
    padding: 0;
    display: inline-block;
}
.scrollin-logo .logo-title {
    font-size: 40px;
    font-weight: bold;
    padding: 10px 17px;
    display: block;
color:#fff;
}
.scrolling-menu {
    float: right;
    display: inline-block;
    width: auto;
}
.scrolling-menu #nav {
    list-style: none;
    margin: 0;
    padding: 0;
    z-index: 999;
}
.scrolling-menu #nav li {
    display: inline-block;
    float: left;
    line-height: 1;
    list-style: none outside none;
   padding: 16px 17px;
    text-align: left;
}
.scrolling-menu #nav li a {
    background: transparent;
    color: #fff;
    display: block;
    font-size: 15px;
    padding: 0 0 8px;
    position: relative;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 1.3px;
}
.scrolling-menu #nav li a:hover {
    color: $maincolor;
}
.scrolling-menu #nav li.current a {
  color: $maincolor;
}
.scrolling-menu #nav li.current a:before {
    position: absolute;
    bottom: 0;
    left: 0;
   width: 100%;
    opacity: 1;
    height: 1px;
    content: '';
    -webkit-transition: all ease .3s;
    transition: all ease .3s;
    background: $maincolor;
}
/* ######## Navigation Menu Css ######################### */
.slicknav_menu {
display:none;
}

.tm-menu .slicknav_menu {
right:0;
display:none;
}

.scrolling-menu .slicknav_menu {
right:0;
}
.slicknav_menu {
padding:0 10px;
    position: absolute;
    z-index: 9;
}
.slicknav_menu .slicknav_icon-bar {
background-color: #343434;
}
.index .slicknav_menu .slicknav_icon-bar {
background-color: #fff;
}
.slicknav_nav a{
padding:5px 10px;
margin:2px 5px;
text-decoration:none;
color:#000;
font-size:11px;
font-weight:400;
letter-spacing:2px;
text-transform:uppercase;

}
/*
    Mobile Menu Core Style
*/

.slicknav_btn { position: relative; display: block; vertical-align: middle; float: right;  line-height: 27px; cursor: pointer;  height:27px;}
.slicknav_menu  .slicknav_menutxt { display: block; line-height: 1.188em; float: left; }
.slicknav_menu .slicknav_icon { float: left; margin: 0.188em 0 0 0.438em; }
.slicknav_menu .slicknav_no-text { margin: 0 }
.slicknav_menu .slicknav_icon-bar { display: block; width: 1.125em; height: 0.125em; }
.slicknav_btn .slicknav_icon-bar + .slicknav_icon-bar { margin-top: 0.188em }
.slicknav_nav { clear: both }
.slicknav_nav ul,
.slicknav_nav li { display: block }
.slicknav_nav .slicknav_arrow { font-size: 0.8em; margin: 0 0 0 0.4em; }
.slicknav_nav .slicknav_item { cursor: pointer; }
.slicknav_nav .slicknav_row { display: block; }
.slicknav_nav a { display: block }
.slicknav_nav .slicknav_item a,
.slicknav_nav .slicknav_parent-link a { display: inline }
.slicknav_menu:before,
.slicknav_menu:after { content: " "; display: table; }
.slicknav_menu:after { clear: both }
.scroll-header.scrolled-header .slicknav_btn {color:#fff;}
.scroll-header.scrolled-header .slicknav_menu .slicknav_icon-bar {
    background-color: #fff;
}
/* IE6/7 support */
.slicknav_menu { *zoom: 1 }

/* 
    User Default Style
    Change the following styles to modify the appearance of the menu.
*/

.slicknav_menu {
    font-size:16px;
}
/* Button */
.slicknav_btn {
    margin: 5px 5px 6px;
    text-decoration:none;
    text-shadow: 0 1px 1px rgba(255, 255, 255, 0.75);
    -webkit-border-radius: 4px;
    -moz-border-radius: 4px;
    border-radius: 4px;  
    
}
/* Button Text */
.slicknav_menu  .slicknav_menutxt {
    color: #FFF;
    font-weight: bold;
    text-shadow: 0 1px 3px #000;
}
/* Button Lines */


.slicknav_nav {
    color:#fff;
    margin:0;
    padding:0;
    font-size:0.875em;
background: #fff;

}
.slicknav_nav, .slicknav_nav ul {
    list-style: none;
    overflow:hidden;
}
.slicknav_nav ul {
    padding:0;
    margin:8px 0 0 20px;
}
.slicknav_nav .slicknav_row {
    padding:5px 10px;
    margin:2px 5px;
}

.slicknav_nav .slicknav_item a,
.slicknav_nav .slicknav_parent-link a {
    padding:0;
    margin:0;
}
.slicknav_nav .slicknav_row:hover {
    
}
.slicknav_nav a:hover{
    color: $maincolor;
}
.slicknav_nav .slicknav_txtnode {
     margin-left:15px;   
}

.slicknav_menu .slicknav_no-text {
	margin-top:15px;
}
.tm-menu {
    font-weight: 400;
    margin: 0;
height:60px;
text-align:center;
     float: right;
   display: inline-block;
    width: auto;
}

ul#nav1 {
    list-style: none;
    margin: 0;
    padding: 0;
text-align: center;
}
#menu .widget {
    display: none;
}
#menu {
    height: 60px;
    position: relative;
    text-align: center;
    z-index: 15;
margin:0 auto;
}
.menu-wrap {
margin:0 auto;
position: relative;
}
#menu ul > li {
    position: relative;
    vertical-align: middle;
    display: inline-block;
    padding: 0;
    margin: 0;
}
#menu ul > li:hover > a {
    color: $maincolor
}
.index #menu ul > li > a {
color:#fff;
}
#menu ul > li > a {
    color: #000;
    font-size: 14px;
    line-height: 60px;
    display: inline-block;
    text-transform: uppercase;
    text-decoration: none;
    letter-spacing: 1px;
    margin: 0;
    padding: 0 12px;

}
.scroll-header.scrolled-header #menu ul > li > a, .scroll-header.scrolled-header #header h1 a {
color:#fff;
}
.scroll-header.scrolled-header #menu ul > li > ul > li > a {
color:#000;
}
#menu ul > li:first-child > a {
    padding-left: 0;
}

#menu ul > li > ul > li:first-child > a:before, #menu ul > li > ul > li > ul > li:first-child > a:before {
display:none;
}
#menu ul > li > ul > li:first-child > a {
    padding-left: 12px
}
#menu ul > li > ul {
    position: absolute;
    background: #fff;
    -webkit-box-shadow: 0 7px 7px rgba(0, 0, 0, 0.15);
    -moz-box-shadow: 0 7px 7px rgba(0, 0, 0, 0.15);
    box-shadow: 0 7px 7px rgba(0, 0, 0, 0.15);
    top: 100%;
    left: 0;
    min-width: 180px;
    padding: 0;
    z-index: 99;
    margin-top: 0;
    visibility: hidden;
    opacity: 0;
   webkit-transform: translate3d(-11px, 0, 0);
    transform: translate3d(-11px, 0, 0);
    -webkit-animation-duration: .5s;
    animation-duration: .5s;
}
#menu ul > li > ul > li > ul {
    position: absolute;
    top: 0;
    left: 180px;
    width: 180px;
    background: #fff;
    z-index: 99;
    margin-top: 0;
    margin-left: 0;
    padding: 0;
    border-left: 1px solid #e5e5e5;
    visibility: hidden;
    opacity: 0;
    -webkit-transform: translateY(10px);
    -moz-transform: translateY(10px);
    transform: translateY(10px)
}
#menu ul > li > ul > li {
    display: block;
    float: none;
    text-align: left;
    position: relative;
border-bottom: 1px solid;
    border-top: none;
    border-color: #e5e5e5;
}
#menu ul > li > ul > li:hover {
    background-color: rgba(255, 255, 255, 0.03)
}
#menu ul > li > ul > li a {
    font-size: 11px;
    display: block;
    color: #000;
    line-height: 35px;
    text-transform: uppercase;
    text-decoration: none;
    margin: 0;
    padding: 0 12px;
    border-right: 0;
    border: 0
}
.index #menu ul > li > ul > li a {
color:#000;
}
#menu ul > li.parent > a:after {
    content: '\f107';
    font-family: FontAwesome;
    float: right;
    margin-left: 5px
}
#menu ul > li:hover > ul,
#menu ul > li > ul > li:hover > ul {
    opacity: 1;
    visibility: visible;
    -webkit-transform: translateY(0);
    -moz-transform: translateY(0);
    transform: translateY(0)
}
#menu ul > li > ul > li.parent > a:after {
    content: '\f105';
    float: right
}
#menu ul ul {

}

/* ######## Header Css ######################### */
#header-wrapper {
text-align: center;
padding:0;
    margin-bottom: 10px;
box-sizing:border-box;
position:relative;
    width: 100%;
}
.background-container{
  position: relative;
height:380px;
overflow:hidden;
background: $maincolor url(//4.bp.blogspot.com/-cz0BYywT9k4/WgGMWiiCEDI/AAAAAAAAEK0/YeAuNhf_LOoprntp89SozkFS5BwPhbR7QCK4BGAYYCw/s1600/head-back.jpg) no-repeat;
    background-attachment: fixed;
    background-size: cover;
background-position:bottom center;
}


.index #header-wrapper {
margin-bottom:0;
}
.item .header-logo-desc p, .static_page .header-logo-desc p, .error_page .header-logo-desc p, .item .top-bar-social #social a, .static_page .top-bar-social #social a, .error_page .top-bar-social #social a {
   color:#303030;
}
.item #header-wrapper, .static_page #header-wrapper, .error_page #header-wrapper {
    background: #fff;
    height: auto;
border-bottom: 1px solid #eee;
    box-shadow: 0 -2px 19px rgba(0,0,0,.1);
    padding-bottom: 15px;
}

#header {
padding: 0;
}
#header-inner {
text-align: center;
display: inline-block;
}
#header h1 {
    color: #fff;
    margin: 0;
    font-size: 40px;
    line-height: 1.4em;
    text-transform: Uppercase;
    letter-spacing: 1px;
}
#header .description {
    display:none;
}
.sora-author-box {
    padding: 57px 50px 15px 50px;
    box-sizing: border-box;
    overflow: hidden;
}
.sora-author-box-image {
width:40%;
  float: left;
    margin-right: 5%;
    margin-bottom: 10px;
}
.sora-author-box-image img {
    height: 385px;
    object-fit: cover;
}
.sora-author-box-text {
    padding: 0;
    overflow: hidden;
    text-align: left;
}
.sora-author-box-text-head {
    color: #3d4451;
    padding-bottom: 25px;
    margin-bottom: 25px;
    border-bottom: 1px solid #dedede;
}
.sora-author-box-text .hello-txt {
   background-color: $maincolor;
color: #fff;
    font-size: 14px;
    font-weight: 700;
    line-height: 1.1;
    display: inline-block;
    padding: 7px 12px;
    text-transform: uppercase;
    position: relative;
    margin-bottom: 28px;
}
.sora-author-box-text .hello-txt:before {
border-left-color:$maincolor;
content: '';
    width: 0;
    height: 0;
    top: 100%;
    left: 5px;
    display: block;
    position: absolute;
    border-style: solid;
    border-width: 0 0 8px 8px;
}
.sora-author-box-text .profile-title {
   font-size: 36px;
    line-height: 1.1;
    font-weight: 700;
    margin-bottom: 5px;
color:#3d4451;
}
.sora-author-box-text .profile-title span {
font-weight: 300;
}
.sora-author-box-text .profile-position {
    font-size: 18px;
    font-weight: 400;
    line-height: 1.1;
    margin-bottom: 0;
}
.sora-author-box-text-details ul {
margin: 0;
    padding: 0;
    list-style: none;
}
.sora-author-box-text-details .profile-list li {
    margin-bottom: 13px;
  list-style: none;
padding:0;
}
.sora-author-box-text-details .profile-list li .list-title {
    display: block;
    width: 120px;
    float: left;
    color: #333333;
    font-size: 12px;
    font-weight: 700;
    line-height: 20px;
    text-transform: uppercase;
}
.sora-author-box-text-details .profile-list li .cont {
    display: block;
    margin-left: 125px;
    font-size: 15px;
    font-weight: 400;
    line-height: 20px;
    color: #9da0a7;
}
.sora-author-box-text-details .profile-list li .list-button {
    color: #fff;
    font-size: 12px;
    font-weight: 700;
    line-height: 1;
    text-transform: none;
    padding: 5px 8px;
    display: inline-block;
    position: relative;
    top: -2px;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    border-radius: 3px;
background:$maincolor;
}
.sora-author-box-text-details .profile-list li .fa {
    margin-right: 10px;
    vertical-align: baseline;
}
.fenix-head {
 
}
.fenix-sub-head {
margin:0 auto;
    background: #fff;
    margin-top: -270px;
    position: relative;
    z-index: 9;
box-shadow: 0 1px 6px rgba(0, 0, 0, 0.12), 0 1px 4px rgba(0, 0, 0, 0.24);
}
.hero-row {
width:940px;
}
.index .fenix-sub-head, .archive .fenix-sub-head {

}
.fenix-sub-head .social-head {
    padding: 15px 0;
    background: $maincolor;
    box-sizing: border-box;
}
.top-bar-social {
padding: 0;
}
.top-bar-social li {
display: inline-block;
    float: none;
padding: 0;
margin-right: 5px;
}
.top-bar-social li:last-child {
margin-right:0;
}
.top-bar-social .widget ul {
padding: 0;
}
.top-bar-social .LinkList ul {
text-align: center;
margin: 0 0 0 0;
}
.top-bar-social #social a {
display: block;
width: 40px;
height: 40px;
line-height: 40px;
font-size: 18px;
color: $maincolor;
background:#fff;
border: 1px solid #e4e4e4;
transition: all 0.3s linear;
-moz-transition: all 0.3s linear;
-webkit-transition: all 0.3s linear;
-o-transition: all 0.3s linear;
}
.top-bar-social #social a:before {
display: inline-block;
font: normal normal normal 22px/1 FontAwesome;
font-size: inherit;
font-style: normal;
font-weight: 400;
-webkit-font-smoothing: antialiased;
-moz-osx-font-smoothing: grayscale;
}
.top-bar-social .bloglovin:before{content:"\f004"}
.top-bar-social .facebook:before{content:"\f09a"}
.top-bar-social .twitter:before{content:"\f099"}
.top-bar-social .gplus:before{content:"\f0d5"}
.top-bar-social .rss:before{content:"\f09e"}
.top-bar-social .youtube:before{content:"\f167"}
.top-bar-social .skype:before{content:"\f17e"}
.top-bar-social .stumbleupon:before{content:"\f1a4"}
.top-bar-social .tumblr:before{content:"\f173"}
.top-bar-social .vine:before{content:"\f1ca"}
.top-bar-social .stack-overflow:before{content:"\f16c"}
.top-bar-social .linkedin:before{content:"\f0e1"}
.top-bar-social .dribbble:before{content:"\f17d"}
.top-bar-social .soundcloud:before{content:"\f1be"}
.top-bar-social .behance:before{content:"\f1b4"}
.top-bar-social .digg:before{content:"\f1a6"}
.top-bar-social .instagram:before{content:"\f16d"}
.top-bar-social .pinterest:before{content:"\f0d2"}
.top-bar-social .delicious:before{content:"\f1a5"}
.top-bar-social .codepen:before{content:"\f1cb"}

.top-bar-social ul#social a:hover {
border-radius: 50%;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.sora-cv-author-details {
    margin: 15px auto;
    position: relative;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
background-color: #fff;
    transition: box-shadow .25s;
    -webkit-transition: box-shadow .25s;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.sora-cv-author-details .card-content {
    padding: 40px;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}
.sora-cv-author-details .card-content p {
color: #000;
    font-size: 18px;
    font-weight: 300;
    line-height: 1.8;
    text-align: center;
}
.sora-cv-author-details .card-action {
    border-top: 1px solid rgba(160, 160, 160, .2);
    padding: 20px;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}
.sora-cv-author-details .card-action .about-btn {
    height: auto;
    margin-right: auto;
    margin-left: auto;
    animation-delay: 1s;
    text-align: center;
}
.sora-cv-author-details .card-action .about-btn .btn {
    margin: 7px 7px;
    background: $maincolor;
    color: #fff;
    width: 180px;
    border-radius: 2px;
    display: inline-block;
    padding: 6px 12px;
    font-size: 14px;
    font-weight: 400;
    line-height: 1.42857143;
    text-align: center;
    white-space: nowrap;
    vertical-align: middle;
    -ms-touch-action: manipulation;
    touch-action: manipulation;
    cursor: pointer;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
position: relative;
    overflow: hidden;
    z-index: 1;
    will-change: opacity, transform;
    transition: all .3s ease-out;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
/* ######## Skill Css ######################### */
.skill-wrapper {
    text-align: center;
}
.skill-wrapper .skill-progress {
  display: inline-block;
  background-color: rgba(141, 166, 179, 0.4);
  width: 120px;
  height: 120px;
  border-radius: 50%;
  margin-right: 25px;
}
.skill-wrapper .skill-progress:last-child {
  margin-right: 0;
}
.skill-wrapper .skill-progress .circle .mask, .skill-wrapper .skill-progress .circle .mask:before {
  width: 120px;
  height: 120px;
  position: absolute;
  border-radius: 50%;
  transition: -webkit-transform 2s;
  transition: -ms-transform 2s;
  transition: transform 2s;
  -webkit-backface-visibility: hidden;
  clip: rect(0px, 120px, 120px, 60px);
}
.skill-wrapper .skill-progress .circle .mask:before {
  display: block;
  content: '';
  clip: rect(0px, 60px, 120px, 0px);
  background-color: $maincolor;
}
.skill-wrapper .skill-progress .circle:before {
  content: '';
  display: block;
  width: 120px;
  height: 120px;
  position: absolute;
  border-radius: 50%;
  box-shadow: 6px 6px 10px rgba(0, 0, 0, 0.3) inset;
}
.skill-wrapper .skill-progress .inset {
  width: 85px;
  height: 85px;
  position: absolute;
  margin-left: 17.5px;
  margin-top: 17.5px;
  background-color: #fbfbfb;
  border-radius: 50%;
  box-shadow: 6px 6px 10px rgba(0, 0, 0, 0.3);
}
.skill-wrapper .skill-progress .inset:before {
  content: '';
  display: block;
  width: 44px;
  height: 22px;
  position: absolute;
  top: 31.5px;
  left: 20.5px;
  line-height: 1;
  transition: width 2s 3s;
  overflow: hidden;
}
.skill-wrapper .skill-progress .inset .numbers {
  margin-top: -22px;
  transition: width 2s;
}

.go:nth-child(n+1) .circle .mask:before, .go:nth-child(n+1) .circle .mask:nth-child(2), .go:nth-child(n+1) .skill-wrapper .skill-progress .circle .mask:nth-child(2):before, .skill-wrapper .skill-progress .go:nth-child(n+1) .circle .mask:nth-child(2):before {
  -webkit-transform: rotate(153deg);
  -ms-transform: rotate(153deg);
  transform: rotate(153deg);
}
.go:nth-child(n+1) .inset .numbers {
  width: 3784px;
}
.go:nth-child(n+1) .inset .numbers:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "85%";
  font-size: 22px;
  font-weight: 800;
  color: #455fae;
  animation: go-1 2s ease-out;
}
@keyframes go-1 {
  1.17647% {
    content: "1%";
  }
  2.35294% {
    content: "2%";
  }
  3.52941% {
    content: "3%";
  }
  4.70588% {
    content: "4%";
  }
  5.88235% {
    content: "5%";
  }
  7.05882% {
    content: "6%";
  }
  8.23529% {
    content: "7%";
  }
  9.41176% {
    content: "8%";
  }
  10.58824% {
    content: "9%";
  }
  11.76471% {
    content: "10%";
  }
  12.94118% {
    content: "11%";
  }
  14.11765% {
    content: "12%";
  }
  15.29412% {
    content: "13%";
  }
  16.47059% {
    content: "14%";
  }
  17.64706% {
    content: "15%";
  }
  18.82353% {
    content: "16%";
  }
  20% {
    content: "17%";
  }
  21.17647% {
    content: "18%";
  }
  22.35294% {
    content: "19%";
  }
  23.52941% {
    content: "20%";
  }
  24.70588% {
    content: "21%";
  }
  25.88235% {
    content: "22%";
  }
  27.05882% {
    content: "23%";
  }
  28.23529% {
    content: "24%";
  }
  29.41176% {
    content: "25%";
  }
  30.58824% {
    content: "26%";
  }
  31.76471% {
    content: "27%";
  }
  32.94118% {
    content: "28%";
  }
  34.11765% {
    content: "29%";
  }
  35.29412% {
    content: "30%";
  }
  36.47059% {
    content: "31%";
  }
  37.64706% {
    content: "32%";
  }
  38.82353% {
    content: "33%";
  }
  40% {
    content: "34%";
  }
  41.17647% {
    content: "35%";
  }
  42.35294% {
    content: "36%";
  }
  43.52941% {
    content: "37%";
  }
  44.70588% {
    content: "38%";
  }
  45.88235% {
    content: "39%";
  }
  47.05882% {
    content: "40%";
  }
  48.23529% {
    content: "41%";
  }
  49.41176% {
    content: "42%";
  }
  50.58824% {
    content: "43%";
  }
  51.76471% {
    content: "44%";
  }
  52.94118% {
    content: "45%";
  }
  54.11765% {
    content: "46%";
  }
  55.29412% {
    content: "47%";
  }
  56.47059% {
    content: "48%";
  }
  57.64706% {
    content: "49%";
  }
  58.82353% {
    content: "50%";
  }
  60% {
    content: "51%";
  }
  61.17647% {
    content: "52%";
  }
  62.35294% {
    content: "53%";
  }
  63.52941% {
    content: "54%";
  }
  64.70588% {
    content: "55%";
  }
  65.88235% {
    content: "56%";
  }
  67.05882% {
    content: "57%";
  }
  68.23529% {
    content: "58%";
  }
  69.41176% {
    content: "59%";
  }
  70.58824% {
    content: "60%";
  }
  71.76471% {
    content: "61%";
  }
  72.94118% {
    content: "62%";
  }
  74.11765% {
    content: "63%";
  }
  75.29412% {
    content: "64%";
  }
  76.47059% {
    content: "65%";
  }
  77.64706% {
    content: "66%";
  }
  78.82353% {
    content: "67%";
  }
  80% {
    content: "68%";
  }
  81.17647% {
    content: "69%";
  }
  82.35294% {
    content: "70%";
  }
  83.52941% {
    content: "71%";
  }
  84.70588% {
    content: "72%";
  }
  85.88235% {
    content: "73%";
  }
  87.05882% {
    content: "74%";
  }
  88.23529% {
    content: "75%";
  }
  89.41176% {
    content: "76%";
  }
  90.58824% {
    content: "77%";
  }
  91.76471% {
    content: "78%";
  }
  92.94118% {
    content: "79%";
  }
  94.11765% {
    content: "80%";
  }
  95.29412% {
    content: "81%";
  }
  96.47059% {
    content: "82%";
  }
  97.64706% {
    content: "83%";
  }
  98.82353% {
    content: "84%";
  }
  100% {
    content: "85%";
  }
}
.go:nth-child(n+1) .inset .numbers:after {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "HTML5";
  font-weight: 100;
  color: #1a2a46;
  top: 120px;
width:120px;
}
.go:nth-child(n+2) .circle .mask:before, .go:nth-child(n+2) .circle .mask:nth-child(2), .go:nth-child(n+2) .skill-wrapper .skill-progress .circle .mask:nth-child(2):before, .skill-wrapper .skill-progress .go:nth-child(n+2) .circle .mask:nth-child(2):before {
  -webkit-transform: rotate(167.4deg);
  -ms-transform: rotate(167.4deg);
  transform: rotate(167.4deg);
}
.go:nth-child(n+2) .inset .numbers {
  width: 4136px;
}
.go:nth-child(n+2) .inset .numbers:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "93%";
  font-size: 22px;
  font-weight: 800;
  color: #455fae;
  animation: go-2 2s ease-out;
}
@keyframes go-2 {
  1.07527% {
    content: "1%";
  }
  2.15054% {
    content: "2%";
  }
  3.22581% {
    content: "3%";
  }
  4.30108% {
    content: "4%";
  }
  5.37634% {
    content: "5%";
  }
  6.45161% {
    content: "6%";
  }
  7.52688% {
    content: "7%";
  }
  8.60215% {
    content: "8%";
  }
  9.67742% {
    content: "9%";
  }
  10.75269% {
    content: "10%";
  }
  11.82796% {
    content: "11%";
  }
  12.90323% {
    content: "12%";
  }
  13.97849% {
    content: "13%";
  }
  15.05376% {
    content: "14%";
  }
  16.12903% {
    content: "15%";
  }
  17.2043% {
    content: "16%";
  }
  18.27957% {
    content: "17%";
  }
  19.35484% {
    content: "18%";
  }
  20.43011% {
    content: "19%";
  }
  21.50538% {
    content: "20%";
  }
  22.58065% {
    content: "21%";
  }
  23.65591% {
    content: "22%";
  }
  24.73118% {
    content: "23%";
  }
  25.80645% {
    content: "24%";
  }
  26.88172% {
    content: "25%";
  }
  27.95699% {
    content: "26%";
  }
  29.03226% {
    content: "27%";
  }
  30.10753% {
    content: "28%";
  }
  31.1828% {
    content: "29%";
  }
  32.25806% {
    content: "30%";
  }
  33.33333% {
    content: "31%";
  }
  34.4086% {
    content: "32%";
  }
  35.48387% {
    content: "33%";
  }
  36.55914% {
    content: "34%";
  }
  37.63441% {
    content: "35%";
  }
  38.70968% {
    content: "36%";
  }
  39.78495% {
    content: "37%";
  }
  40.86022% {
    content: "38%";
  }
  41.93548% {
    content: "39%";
  }
  43.01075% {
    content: "40%";
  }
  44.08602% {
    content: "41%";
  }
  45.16129% {
    content: "42%";
  }
  46.23656% {
    content: "43%";
  }
  47.31183% {
    content: "44%";
  }
  48.3871% {
    content: "45%";
  }
  49.46237% {
    content: "46%";
  }
  50.53763% {
    content: "47%";
  }
  51.6129% {
    content: "48%";
  }
  52.68817% {
    content: "49%";
  }
  53.76344% {
    content: "50%";
  }
  54.83871% {
    content: "51%";
  }
  55.91398% {
    content: "52%";
  }
  56.98925% {
    content: "53%";
  }
  58.06452% {
    content: "54%";
  }
  59.13978% {
    content: "55%";
  }
  60.21505% {
    content: "56%";
  }
  61.29032% {
    content: "57%";
  }
  62.36559% {
    content: "58%";
  }
  63.44086% {
    content: "59%";
  }
  64.51613% {
    content: "60%";
  }
  65.5914% {
    content: "61%";
  }
  66.66667% {
    content: "62%";
  }
  67.74194% {
    content: "63%";
  }
  68.8172% {
    content: "64%";
  }
  69.89247% {
    content: "65%";
  }
  70.96774% {
    content: "66%";
  }
  72.04301% {
    content: "67%";
  }
  73.11828% {
    content: "68%";
  }
  74.19355% {
    content: "69%";
  }
  75.26882% {
    content: "70%";
  }
  76.34409% {
    content: "71%";
  }
  77.41935% {
    content: "72%";
  }
  78.49462% {
    content: "73%";
  }
  79.56989% {
    content: "74%";
  }
  80.64516% {
    content: "75%";
  }
  81.72043% {
    content: "76%";
  }
  82.7957% {
    content: "77%";
  }
  83.87097% {
    content: "78%";
  }
  84.94624% {
    content: "79%";
  }
  86.02151% {
    content: "80%";
  }
  87.09677% {
    content: "81%";
  }
  88.17204% {
    content: "82%";
  }
  89.24731% {
    content: "83%";
  }
  90.32258% {
    content: "84%";
  }
  91.39785% {
    content: "85%";
  }
  92.47312% {
    content: "86%";
  }
  93.54839% {
    content: "87%";
  }
  94.62366% {
    content: "88%";
  }
  95.69892% {
    content: "89%";
  }
  96.77419% {
    content: "90%";
  }
  97.84946% {
    content: "91%";
  }
  98.92473% {
    content: "92%";
  }
  100% {
    content: "80%";
  }
}
.go:nth-child(n+2) .inset .numbers:after {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "CSS/Javascript";
  font-weight: 100;
  color: #1a2a46;
  top: 120px;
}
.go:nth-child(n+3) .circle .mask:before, .go:nth-child(n+3) .circle .mask:nth-child(2), .go:nth-child(n+3) .skill-wrapper .skill-progress .circle .mask:nth-child(2):before, .skill-wrapper .skill-progress .go:nth-child(n+3) .circle .mask:nth-child(2):before {
  -webkit-transform: rotate(156.6deg);
  -ms-transform: rotate(156.6deg);
  transform: rotate(156.6deg);
}
.go:nth-child(n+3) .inset .numbers {
  width: 3872px;
}
.go:nth-child(n+3) .inset .numbers:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "87%";
  font-size: 22px;
  font-weight: 800;
  color: #455fae;
  animation: go-3 2s ease-out;
}
@keyframes go-3 {
  1.14943% {
    content: "1%";
  }
  2.29885% {
    content: "2%";
  }
  3.44828% {
    content: "3%";
  }
  4.5977% {
    content: "4%";
  }
  5.74713% {
    content: "5%";
  }
  6.89655% {
    content: "6%";
  }
  8.04598% {
    content: "7%";
  }
  9.1954% {
    content: "8%";
  }
  10.34483% {
    content: "9%";
  }
  11.49425% {
    content: "10%";
  }
  12.64368% {
    content: "11%";
  }
  13.7931% {
    content: "12%";
  }
  14.94253% {
    content: "13%";
  }
  16.09195% {
    content: "14%";
  }
  17.24138% {
    content: "15%";
  }
  18.3908% {
    content: "16%";
  }
  19.54023% {
    content: "17%";
  }
  20.68966% {
    content: "18%";
  }
  21.83908% {
    content: "19%";
  }
  22.98851% {
    content: "20%";
  }
  24.13793% {
    content: "21%";
  }
  25.28736% {
    content: "22%";
  }
  26.43678% {
    content: "23%";
  }
  27.58621% {
    content: "24%";
  }
  28.73563% {
    content: "25%";
  }
  29.88506% {
    content: "26%";
  }
  31.03448% {
    content: "27%";
  }
  32.18391% {
    content: "28%";
  }
  33.33333% {
    content: "29%";
  }
  34.48276% {
    content: "30%";
  }
  35.63218% {
    content: "31%";
  }
  36.78161% {
    content: "32%";
  }
  37.93103% {
    content: "33%";
  }
  39.08046% {
    content: "34%";
  }
  40.22989% {
    content: "35%";
  }
  41.37931% {
    content: "36%";
  }
  42.52874% {
    content: "37%";
  }
  43.67816% {
    content: "38%";
  }
  44.82759% {
    content: "39%";
  }
  45.97701% {
    content: "40%";
  }
  47.12644% {
    content: "41%";
  }
  48.27586% {
    content: "42%";
  }
  49.42529% {
    content: "43%";
  }
  50.57471% {
    content: "44%";
  }
  51.72414% {
    content: "45%";
  }
  52.87356% {
    content: "46%";
  }
  54.02299% {
    content: "47%";
  }
  55.17241% {
    content: "48%";
  }
  56.32184% {
    content: "49%";
  }
  57.47126% {
    content: "50%";
  }
  58.62069% {
    content: "51%";
  }
  59.77011% {
    content: "52%";
  }
  60.91954% {
    content: "53%";
  }
  62.06897% {
    content: "54%";
  }
  63.21839% {
    content: "55%";
  }
  64.36782% {
    content: "56%";
  }
  65.51724% {
    content: "57%";
  }
  66.66667% {
    content: "58%";
  }
  67.81609% {
    content: "59%";
  }
  68.96552% {
    content: "60%";
  }
  70.11494% {
    content: "61%";
  }
  71.26437% {
    content: "62%";
  }
  72.41379% {
    content: "63%";
  }
  73.56322% {
    content: "64%";
  }
  74.71264% {
    content: "65%";
  }
  75.86207% {
    content: "66%";
  }
  77.01149% {
    content: "67%";
  }
  78.16092% {
    content: "68%";
  }
  79.31034% {
    content: "69%";
  }
  80.45977% {
    content: "70%";
  }
  81.6092% {
    content: "71%";
  }
  82.75862% {
    content: "72%";
  }
  83.90805% {
    content: "73%";
  }
  85.05747% {
    content: "74%";
  }
  86.2069% {
    content: "75%";
  }
  87.35632% {
    content: "76%";
  }
  88.50575% {
    content: "77%";
  }
  89.65517% {
    content: "78%";
  }
  90.8046% {
    content: "79%";
  }
  91.95402% {
    content: "80%";
  }
  93.10345% {
    content: "81%";
  }
  94.25287% {
    content: "82%";
  }
  95.4023% {
    content: "83%";
  }
  96.55172% {
    content: "84%";
  }
  97.70115% {
    content: "85%";
  }
  98.85057% {
    content: "86%";
  }
  100% {
    content: "77%";
  }
}
.go:nth-child(n+3) .inset .numbers:after {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "Python";
  font-weight: 100;
  color: #1a2a46;
  top: 120px;
}
.go:nth-child(n+4) .circle .mask:before, .go:nth-child(n+4) .circle .mask:nth-child(2), .go:nth-child(n+4) .skill-wrapper .skill-progress .circle .mask:nth-child(2):before, .skill-wrapper .skill-progress .go:nth-child(n+4) .circle .mask:nth-child(2):before {
  -webkit-transform: rotate(100.8deg);
  -ms-transform: rotate(100.8deg);
  transform: rotate(100.8deg);
}
.go:nth-child(n+4) .inset .numbers {
  width: 2508px;
}
.go:nth-child(n+4) .inset .numbers:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "56%";
  font-size: 22px;
  font-weight: 800;
  color: #455fae;
  animation: go-4 2s ease-out;
}
@keyframes go-4 {
  1.78571% {
    content: "1%";
  }
  3.57143% {
    content: "2%";
  }
  5.35714% {
    content: "3%";
  }
  7.14286% {
    content: "4%";
  }
  8.92857% {
    content: "5%";
  }
  10.71429% {
    content: "6%";
  }
  12.5% {
    content: "7%";
  }
  14.28571% {
    content: "8%";
  }
  16.07143% {
    content: "9%";
  }
  17.85714% {
    content: "10%";
  }
  19.64286% {
    content: "11%";
  }
  21.42857% {
    content: "12%";
  }
  23.21429% {
    content: "13%";
  }
  25% {
    content: "14%";
  }
  26.78571% {
    content: "15%";
  }
  28.57143% {
    content: "16%";
  }
  30.35714% {
    content: "17%";
  }
  32.14286% {
    content: "18%";
  }
  33.92857% {
    content: "19%";
  }
  35.71429% {
    content: "20%";
  }
  37.5% {
    content: "21%";
  }
  39.28571% {
    content: "22%";
  }
  41.07143% {
    content: "23%";
  }
  42.85714% {
    content: "24%";
  }
  44.64286% {
    content: "25%";
  }
  46.42857% {
    content: "26%";
  }
  48.21429% {
    content: "27%";
  }
  50% {
    content: "28%";
  }
  51.78571% {
    content: "29%";
  }
  53.57143% {
    content: "30%";
  }
  55.35714% {
    content: "31%";
  }
  57.14286% {
    content: "32%";
  }
  58.92857% {
    content: "33%";
  }
  60.71429% {
    content: "34%";
  }
  62.5% {
    content: "35%";
  }
  64.28571% {
    content: "36%";
  }
  66.07143% {
    content: "37%";
  }
  67.85714% {
    content: "38%";
  }
  69.64286% {
    content: "39%";
  }
  71.42857% {
    content: "40%";
  }
  73.21429% {
    content: "41%";
  }
  75% {
    content: "42%";
  }
  76.78571% {
    content: "43%";
  }
  78.57143% {
    content: "44%";
  }
  80.35714% {
    content: "45%";
  }
  82.14286% {
    content: "46%";
  }
  83.92857% {
    content: "47%";
  }
  85.71429% {
    content: "48%";
  }
  87.5% {
    content: "49%";
  }
  89.28571% {
    content: "50%";
  }
  91.07143% {
    content: "51%";
  }
  92.85714% {
    content: "52%";
  }
  94.64286% {
    content: "53%";
  }
  96.42857% {
    content: "54%";
  }
  98.21429% {
    content: "55%";
  }
  100% {
    content: "56%";
  }
}
.go:nth-child(n+4) .inset .numbers:after {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "JS";
  font-weight: 100;
  color: #1a2a46;
  top: 120px;
}
.go:nth-child(n+5) .circle .mask:before, .go:nth-child(n+5) .circle .mask:nth-child(2), .go:nth-child(n+5) .skill-wrapper .skill-progress .circle .mask:nth-child(2):before, .skill-wrapper .skill-progress .go:nth-child(n+5) .circle .mask:nth-child(2):before {
  -webkit-transform: rotate(77.4deg);
  -ms-transform: rotate(77.4deg);
  transform: rotate(77.4deg);
}
.go:nth-child(n+5) .inset .numbers {
  width: 1936px;
}
.go:nth-child(n+5) .inset .numbers:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "43%";
  font-size: 22px;
  font-weight: 800;
  color: #455fae;
  animation: go-5 2s ease-out;
}
@keyframes go-5 {
  2.32558% {
    content: "1%";
  }
  4.65116% {
    content: "2%";
  }
  6.97674% {
    content: "3%";
  }
  9.30233% {
    content: "4%";
  }
  11.62791% {
    content: "5%";
  }
  13.95349% {
    content: "6%";
  }
  16.27907% {
    content: "7%";
  }
  18.60465% {
    content: "8%";
  }
  20.93023% {
    content: "9%";
  }
  23.25581% {
    content: "10%";
  }
  25.5814% {
    content: "11%";
  }
  27.90698% {
    content: "12%";
  }
  30.23256% {
    content: "13%";
  }
  32.55814% {
    content: "14%";
  }
  34.88372% {
    content: "15%";
  }
  37.2093% {
    content: "16%";
  }
  39.53488% {
    content: "17%";
  }
  41.86047% {
    content: "18%";
  }
  44.18605% {
    content: "19%";
  }
  46.51163% {
    content: "20%";
  }
  48.83721% {
    content: "21%";
  }
  51.16279% {
    content: "22%";
  }
  53.48837% {
    content: "23%";
  }
  55.81395% {
    content: "24%";
  }
  58.13953% {
    content: "25%";
  }
  60.46512% {
    content: "26%";
  }
  62.7907% {
    content: "27%";
  }
  65.11628% {
    content: "28%";
  }
  67.44186% {
    content: "29%";
  }
  69.76744% {
    content: "30%";
  }
  72.09302% {
    content: "31%";
  }
  74.4186% {
    content: "32%";
  }
  76.74419% {
    content: "33%";
  }
  79.06977% {
    content: "34%";
  }
  81.39535% {
    content: "35%";
  }
  83.72093% {
    content: "36%";
  }
  86.04651% {
    content: "37%";
  }
  88.37209% {
    content: "38%";
  }
  90.69767% {
    content: "39%";
  }
  93.02326% {
    content: "40%";
  }
  95.34884% {
    content: "41%";
  }
  97.67442% {
    content: "42%";
  }
  100% {
    content: "43%";
  }
}
.go:nth-child(n+5) .inset .numbers:after {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  content: "PHP";
  font-weight: 100;
  color: #1a2a46;
  top: 120px;
}
/* ######## Section 1 Css ######################### */
.sora-special-box {
    overflow: hidden;
    margin: 0 auto;
padding:20px 0;
}
.special-wrap {
    margin: 0 auto;
    position: relative;
}
.special-wrap-inner {
 background-color: #fff;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
 -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    overflow: hidden;
    padding: 20px;
}
.special-title {
    text-align: center;
margin-bottom: 35px;
}
.special-title h4 {
color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
text-transform:uppercase;
}
.special-title h4 .lnr {
margin-right:5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
color:#3498db;
}
.special-tiles {
    width: 100%;
    box-sizing: border-box;
    text-align: left;
    margin-bottom: 20px;
}
.special-icons {
    font-size: 45px;
    float: left;
    color: #303030;
    margin-right: 10px;
width: 50px;
    height: 60px;
    line-height: 60px;
}
.special-heading {
    font-size: 14px;
    line-height: 21px;
    color: #303030;
text-transform: capitalize;
    letter-spacing: 1.5px;
    margin-bottom: 10px;
font-weight:bold;
}
.special-text {
    color: #606060;
}


.skills, .skill-details {
  padding: 15px;
    width: 50%;
    float: left;
    box-sizing: border-box;
    padding-right: 40px;
    padding-left: 0;
}
.skill-details {
float:right;
padding-left: 40px;
    padding-right: 0;
}
.skills dt:after {
  width: 100%;
  background-color: #e0e0e0;
  height: 0.5rem;
  content: "";
  display: block;
}

.skills dd {
  background: red;
  width: 0;
  height: 0.5rem;
  position: relative;
  top: -0.5rem;
}
.skills dd.html {
  background: #F44336;
}
.skills dd.css {
  background: #2196F3;
}
.skills dd.jquery {
  background: #FFCA28;
}
.skills dd.scss {
  background: #F06292;
}
.skills dd.javascript {
  background: #FFA000;
}
.skills dd.php {
  background: #303F9F;
}
.skills dd.xml {
  background: #27ae60;
}
/* ######## Section 2 Css ######################### */
.sora-works-box {
    overflow: hidden;
    margin: 0 auto;
padding:20px 0;
}
.works-wrap {
margin:0 auto;
}
.works-title {
    text-align: center;
margin-bottom: 35px;
}
.works-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.works-title h4 .lnr {
    margin-right: 5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
color:#1abc9c;
}


#timeline {
 
}
.timeline {
   position: relative;
   padding-top: 20px;
   background-color: inherit;
list-style:none;
}

.timeline:after {
   content: '';
   position: absolute;
   width: 5px;
   background-color: $maincolor;
   left: 50%;
   top: 0;
   bottom: 0;
   margin-left: -2px;
}

.timeline--first:after {
   top: 20px;
}

.era {
   text-align: center;
   position: relative;
   z-index: 1;
   padding-bottom: 20px;
list-style:none;
}

.era__title {
   background-color: $maincolor;
   color: #EEEEEE;
   display: inline-block;
   padding: 10px 20px;
   border-radius: 4px;
   cursor: default;
}

.entry {
   padding: 10px 30px 40px 30px;
   width: 50%;
   position: relative;
   background-color: inherit;
list-style:none;
}

.entry--right {
   margin-left: 50%;
}

.entry__content {
   padding: 20px 30px;
   background-color: #fff;
   position: relative;
   border-radius: 4px;
   cursor: default;
   transition: all 0.3s ease 0s;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.entry.entry--left .entry__content {
    border-left: 5px solid $maincolor;
}
.entry.entry--right .entry__content {
    border-right: 5px solid $maincolor;
}
.entry__content:hover {
   background-color: #FFFFFF;
}
.entry__content h2 {
    color: #414141;
    font-size: 22px;
    font-weight: 400;
    line-height: 1.1;
    text-align: center;
    margin-bottom: 20px;
    text-transform: uppercase;
}
.entry__content .date {
    font-size: 16px;
    font-weight: 700;
    line-height: 1;
    text-align: center;
    margin-bottom: 15px;
color:$maincolor;
}
.entry:before {
   content: " ";
   height: 0;
   position: absolute;
   top: 20px;
   width: 0;
   z-index: 1;
}

.entry:after {
   content: '';
   position: absolute;
   width: 23px;
   height: 23px;
   right: -12px;
   background-color: #EEEEEE;
   border: 4px solid $maincolor;
   top: 20px;
   border-radius: 50%;
   z-index: 1;
}

.entry--right:after {
   right: auto;
   left: -12px;
}
/* ######## Testimonial Css ######################### */
/*! Flickity v1.0.0
http://flickity.metafizzy.co
---------------------------------------------- */
.flickity-enabled{position:relative}.flickity-enabled:focus{outline:0}.flickity-viewport{overflow:hidden;position:relative;height:100%}.flickity-slider{position:absolute;width:100%;height:100%}.flickity-enabled.is-draggable{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.flickity-enabled.is-draggable .flickity-viewport{cursor:move;cursor:-webkit-grab;cursor:grab}.flickity-enabled.is-draggable .flickity-viewport.is-pointer-down{cursor:-webkit-grabbing;cursor:grabbing}.flickity-prev-next-button{position:absolute;top:50%;width:44px;height:44px;    border: 1px solid #d7dbde;background:#fff;background:hsla(0,0%,100%,.75);cursor:pointer;-webkit-transform:translateY(-50%);-ms-transform:translateY(-50%);transform:translateY(-50%)}.flickity-prev-next-button:hover{background:#fff}.flickity-prev-next-button:focus{outline:0;box-shadow:0 0 0 5px #09F}.flickity-prev-next-button:active{filter:alpha(opacity=60);opacity:.6}.flickity-prev-next-button.previous{left:10px}.flickity-prev-next-button.next{right:10px}.flickity-rtl .flickity-prev-next-button.previous{left:auto;right:10px}.flickity-rtl .flickity-prev-next-button.next{right:auto;left:10px}.flickity-prev-next-button:disabled{filter:alpha(opacity=30);opacity:.3;cursor:auto}.flickity-prev-next-button svg{position:absolute;left:20%;top:20%;width:60%;height:60%}.flickity-prev-next-button .arrow{fill:#333}.flickity-prev-next-button.no-svg{color:#333;font-size:26px}.flickity-page-dots{position:absolute;width:100%;bottom:-25px;padding:0;margin:0;list-style:none;text-align:center;line-height:1}.flickity-rtl .flickity-page-dots{direction:rtl}.flickity-page-dots .dot{display:inline-block;width:10px;height:10px;margin:0 8px;background:#efefef;border-radius:50%;filter:alpha(opacity=80);opacity:.80;cursor:pointer;    padding: 0;}.flickity-page-dots .dot.is-selected{filter:alpha(opacity=100);opacity:1}
.main-gallery {
background-color: #fff;
    box-shadow: 0 1px 6px rgba(0, 0, 0, 0.12), 0 1px 4px rgba(0, 0, 0, 0.24);

}
.main-gallery-wrap {
margin:0 auto;
}
.gallery-cell {
  width: 100%;
}
.testimonial-title {
    text-align: center;
       margin: 25px 0;
}
.testimonial-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.testimonial-title .lnr {
    margin-right: 5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
    color: #3498db;
}
.testimonial {
     text-align: left;
  max-width: 850px;
  margin: 55px auto 40px auto;
  padding: 0 20px;
}
.testimonial-image {
    float: left;
    margin-right: 22px;
}
.testimonial-avatar {
 width: 53px;
    display: block;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
}
.person-speech {
    font-size: 18px;
    font-weight: 400;
    line-height: 1.4;
    position: relative;
    padding-bottom: 27px;
    border-bottom: 1px solid #dddad9;
}
.testimonial-quote {
  font-size: 22px;
color:#3d4451;
}
.testimonial-quote:before {
    content: "\f10e";
    top: 2px;
    left: -55px;
    position: absolute;
    font-size: 23px;
    line-height: 1;
color:$maincolor;
    display: inline-block;
    font: normal normal normal 22px/1 FontAwesome;
    font-size: inherit;
    font-style: normal;
    font-weight: 400;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
.testimonial-meta {
    padding-top: 25px;
}
.testimonial-author {
     color: #757575;
    font-size: 20px;
    font-weight: 700;
    line-height: 1.1;
    display: block;
    margin-bottom: 3px;
}
.testimonial-author-details{
    color: #d0d0d0;
    font-size: 13px;
    font-weight: 400;
    line-height: 1.1;
    text-transform: uppercase;
}
.flickity-page-dots {
  bottom: 25px;
}

.flickity-page-dots .dot.is-selected {
  background: $maincolor;
}
/* ######## Section 3 Css ######################### */
.sora-about-box {
    background: #f8f8f8;
    overflow: hidden;
    margin: 0 auto;
padding:20px 0;
}
.about-wrap {
margin:0 auto;
}
.about-title {
    text-align: center;
margin-bottom: 35px;
}
.about-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.about-title h4 .lnr {
    margin-right: 5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
    color: #f39c12;
}
.about-tiles {
    width: 33.33%;
    float: left;
    padding: 10px;
    box-sizing: border-box;
    text-align: center;
}
.price_card{
 width: 33.33%;
    box-sizing: border-box;
    text-align: center;	
	 float: left;
	top: 0;
position:relative;
}
.price_card_wrap {
background: rgb(255, 255, 255);
    overflow: hidden;
}
.price_card:not(:last-child){
	padding-right: 20px;
}
.header{
	color: rgb(255, 255, 255);
}
.alpha .header{
	background: rgb(245, 166, 35);
}
.bravo .header{
	background: rgb(246, 77, 77);
}
.charlie .header{
	background: rgb(48, 219, 181);
}
.price{
	width: 100%;
	font-size: 60px;
    line-height: 60px;
	font-weight: 300;
	display: block;
	text-align: center;
	padding: 30px 0 10px;
}
.name{
	width: 100%;
	font-size: 15px;
	font-weight: 700;
	display: block;
	text-align: center;
	padding: 0 0 30px;
}
.features{
	list-style: none;
	text-align: center;
	color: rgb(138, 138, 138);
	margin: 0;
	padding: 0;
}
.features li{
	padding: 20px 15px;
	width: 100%;
list-style:none;
box-sizing:border-box;
}
.features li:not(:last-child){
	border: 1px solid rgb(242, 242, 242);
	border-top: 0;
	border-left: 0;
	border-right: 0;
}
button{
	color: rgb(255, 255, 255);
	border: 0;
	border-radius: 5px;
	height: 40px;
	width: 200px;
	display: block;
	font-weight: 700;
	font-size: 15px;
	text-transform: uppercase;
	margin: 20px auto 35px;
}
.alpha button{
	background: rgb(245, 166, 35);
}
.bravo button{
	background: rgb(246, 77, 77);
}
.charlie button{
	background: rgb(48, 219, 181);
}
.tip{
	font-family: 'Indie Flower';
	position: absolute;
	color: rgb(117, 117, 117);
	margin: 10px 5px;
left:0;
}

/* ######## Contact Form Css ######################### */
div#sora_blogger_cntct_form {
    padding: 50px 0px;
    border-radius: 2px;
    color: #3d4451;
    font-size: 15px;
    font-weight: bold;
    position: relative;
margin:0 auto;
overflow:hidden;
}
div#sora_blogger_cntct_form .wrap-me {
      margin: 0;
    display: block;
    max-width: 500px;
    width: 100%;
    float: left;
    box-sizing: border-box;
   background-color: #fff;
    padding: 40px 40px 5px;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.contact-title {
    text-align: center;
    margin: 25px 0;
}
.contact-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.contact-title h4 .lnr {
    margin-right: 5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
   color:#95a5a6;
}
.contact-title span {
    color: #3d4451;
}
.contact_list_wrapper {
    text-align: center;
}
.contact-list-info {
    list-style: none;
    padding: 0;
    margin: 0;
    text-align: center;
}
.contact_list_wrapper .contact-list-info li {
    padding: 0;
    padding-left: 15px;
    padding-right: 15px;
    display: inline-block;
    line-height: 25px;
    color: #3d4451;
}
.contact_list_wrapper .contact-list-info li i {
    display: inline;
margin-right: 5px;
    font-size: 15px;
    vertical-align: -2px;
    color: #3d4451;
}
.contact_list_wrapper .contact-list-info li p {
 display: inline;
}
input#ContactForm1_contact-form-name, #ContactForm1_contact-form-email, #ContactForm1_contact-form-email:hover, #ContactForm1_contact-form-email:active {
    padding: 5px;
    margin-top: 4px !important;
    box-shadow: none!Important;
    width: 100%;
    max-width: 100%;
  background: transparent !important;
    color: #3d4451;
    border-color: gainsboro !important;
border-width:0 0 1px 0;
    line-height: 1em;
    min-height: 31px;
    margin-bottom: 15px;
    border-radius: 0px;
}
.contact-form-email-message, .contact-form-email-message:active, .contact-form-email-message:hover {
    padding: 5px;
    margin-top: 4px !important;
    box-shadow: none!Important;
    width: 100%;
max-width: 100%;
    line-height: 1em;
    min-height: 80px;
  background: transparent !important;
    color:#3d4451;
    border-color: gainsboro !important;
border-width:0 0 1px 0;
    margin-bottom: 10px;
    border-radius: 0px;
}
/***** Focus *****/
#ContactForm1_contact-form-name:focus, #ContactForm1_contact-form-email:focus, #ContactForm1_contact-form-email-message:focus {
    outline: none;
    background: transparent !important;
    color: #3d4451;
    border-color: $maincolor !important;
border-width:0 0 1px 0;
    box-shadow: none !important;
    transition: all 0.3s ease-in-out !important;
}
/**** Submit button style ****/
.contact-form-button-submit:hover {
    color: #FFFFFF;
    background: $maincolor !important;
color:#000!important;
}
.contact-form-button-submit {
       background: transparent;
    display: table;
    font-size: 17px;
    margin: 0 !important;
    border-radius: 0 !important;
    max-width: 100%;
    width: 100%;
    min-width: 100%;
    height: 32px;
    line-height: 0.5em;
    letter-spacing: 0.5px;
    font-weight: normal;
position:relative;
    cursor: pointer;
    outline: none!important;
    color: #3d4451;
    border: 1px solid gainsboro !important;
    text-align: center;
    padding: 0px 25px;
    text-transform: capitalize;
    transition: all 300ms ease-in-out;
    -webkit-transition: all 300ms ease-in-out;
    -moz-transition: all 300ms ease-in-out;
}

/**** Submit button on Focus ****/
.contact-form-button-submit:focus, .contact-form-button-submit.focus {
  border-color: $maincolor;
  box-shadow: none !important;
color:#000!important;
}
/**** Error message ****/
.contact-form-success-message, .contact-form-success-message-with-border {
  color: #3d4451 !important;
margin-top:55px !important;
}
/**** Submit Button On Success Message ****/
.contact-form-button-submit.disabled, .contact-form-button-submit.disabled:hover, .contact-form-button-submit.disabled:active {
    opacity: 0.9;
}
/****** Success Message *****/
.contact-form-error-message-with-border {
    background: #000000;
    border: 1px solid #5A5A5A;
    bottom: 0;
    box-shadow: none;
    color: #FDFDFD;
    font-size: 15px;
    font-weight: normal;
    line-height: 35px;
    margin-left: 0;
    opacity: 1;
    position: static;
    text-align: center;
    height: 35px;
    margin-top: 60px;
}
.contact-form-cross {
    height: 14px;
    margin: 5px;
    vertical-align: -8.5%;
    float: right;
    width: 14px;
    border-radius: 50px;
    border: 0 !important;
    cursor: pointer;
}
.contact-form-widget {
    max-width: 100%;
}
.contact-form-success-message-with-border {
    font-weight: normal;
    background-color: #000;
    border: 1px solid #FFF;
    color: #FFF;
    line-height: 35px;
    margin-left: 0;
    font-size: 13px;
    opacity: 1;
    position: static;
    text-align: center;
    height: 35px;
    margin-top: 60px;
}
/* Extra Stuff */

div#sora_blogger_cntct_form span.name-bg, div#sora_blogger_cntct_form span.email-bg {
    display: inline-block;
    line-height: 21px;
    width: 100%;
    color: #3d4451;
    padding: 3px 0;
    margin: 0px 0px 4px;
    box-sizing: border-box;
    height: 30px;
    letter-spacing: 1px;
    font-weight: normal;
}
div#sora_blogger_cntct_form span.message-bg {
    display: inline-block;
    line-height: 21px;
    width: 100%;
    color: #3d4451;
    padding: 3px 0;
    box-sizing: border-box;
    height: 30px;
    margin: 0px 0px 4px;
    letter-spacing: 1px;
    font-weight: normal;
}

div#sora_blogger_cntct_form span.send-bg {
    height: 32px;
    display: inline-block;
    float: left;
    transition: all 0.4s ease-in-out !important;
}


div#sora_blogger_cntct_form span.clear-bg {
    display: none;
   
}


input.contact-form-button.contact-form-button-submit.clear-button:hover {
    background-color: #E83434 !important;
}
div#sora_blogger_cntct_form .clear-button {
   display:none;
}
.map-me-full #map {
    width: 100%;
    height: 378px;
}
.map-me {
    margin: 0;
    display: block;
    max-width: 500px;
    width: 100%;
    float: right;
padding: 40px;
    box-sizing: border-box;
}
.map-me .con-title {
    font-weight: 700;
    letter-spacing: -1px;
    line-height: 48px;
    color: #000;
    margin: 0;
    text-transform: capitalize;
}
.map-me .con-text {
    font-weight: 100;
    line-height: 24px;
    color: #555;
margin: 0 0 10px;
}
.map-me .con-list {
list-style-type: none;
    padding: 0;
}
.map-me .con-list li {
list-style-type: none;
    color: #333;
  line-height: 45px;
    margin-bottom: 15px;
    text-transform: capitalize;
font-weight:normal;
}
.map-me .con-list li i {
    font-size: 1em;
    margin-right: 20px;
    padding: 15px;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    background: $maincolor;
    color: #fff;
    border-radius: 50%;
}
/* ######## Sidebar Css ######################### */
.sidebar .widget {
margin-bottom: 20px;
position: relative;
background: #fff none repeat scroll top left;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.sidebar h2 {
font-size: 17px;
line-height: 27px;
color: #000;
padding: 7px 15px;
font-weight: 400;
letter-spacing: 1.5px;
text-transform: uppercase;
position: relative;
text-align: center;
background: #f7f7f7;
    border: 1px solid #f0f0f0;
}
.sidebar .widget-content {
    padding: 10px;
box-sizing:border-box;
}
.sidebar ul,.sidebar li{
list-style-type:none;
margin:0;
}
/* ######## Counter Css ######################### */
.sora-cv-hobby-details {
    margin: 15px auto;
    position: relative;
}
.sora-cv-hobby-details-inner {
 -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    background-color: #fff;
    transition: box-shadow .25s;
    -webkit-transition: box-shadow .25s;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.sora-cv-hobby-details .hobby-title {
    text-align: center;
    margin-bottom: 35px;
}
.sora-cv-hobby-details .hobby-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.sora-cv-hobby-details .hobby-title .lnr {
    margin-right: 5px;
    padding: 10px;
color:#e74c3c;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
}
.sora-cv-hobby-details .card-content {
    padding: 40px;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}
.sora-cv-hobby-details .card-content p {
    color: #000;
    font-size: 18px;
    font-weight: 300;
    line-height: 1.8;
    text-align: center;
}
.sora-cv-hobby-details .card-action {
    border-top: 1px solid rgba(160, 160, 160, .2);
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
overflow: hidden;
}
.sora-cv-hobby-details .card-action ul {
padding:0;
margin:0;
list-style:none;
}
.sora-cv-hobby-details .card-action ul li {
padding:30px;
    margin: 0;
-webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    list-style: none;
    float: left;
    width: 16.6666666667%;
    box-sizing: border-box;
    text-align: center;
color:$maincolor;
}
.sora-cv-hobby-details .card-action ul li.odd {
    background: $maincolor;
color:#fff;
}
.sora-cv-hobby-details .card-action ul li i {
    font-size: 2.2em;
}
.sora-cv-hobby-details .card-action ul li span {
    display: block;
}
/* ######## Post Css ######################### */
.Portfolio-title {
    text-align: center;
       margin: 25px 0;
}
.Portfolio-title h4 {
    color: #3d4451;
    font-size: 34px;
    line-height: 1.2;
    font-weight: 600;
    text-align: center;
    text-transform: uppercase;
}
.Portfolio-title .lnr {
    margin-right: 5px;
    padding: 10px;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
    color: #f1c40f;
}
article {
    padding: 0;
overflow:hidden;
}
.index article, .archive article {
    padding: 20px;
    box-sizing: border-box;
}
.index .post-grid-item, .archive .post-grid-item {
width:33.33%;
float:left;
padding-right:15px;
box-sizing:border-box;
margin-bottom:15px;
}
.index .post-grid-item:nth-child(3n), .archive .post-grid-item:nth-child(3n) {
padding-right:0;
}
.index .post, .archive .post {
box-shadow: 0 1px 6px rgba(0, 0, 0, 0.12), 0 1px 4px rgba(0, 0, 0, 0.24);
}
.post {
    display: block;
    word-wrap: break-word;
background: #ffffff;
}
.item .post, .static_page .post {
padding: 10px;
    box-sizing: border-box;
box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
overflow:hidden;
}
.home-post-head {
    text-align: center;
}
.post h1 {
    color: #0a0a0a;
    font-size: 28px;
    font-weight: 400;
    line-height: 32px;
    margin: 0 0 10px;
}
.post h2 {
margin-bottom: 12px;
font-size: 20px;
    line-height: 1.3;
    font-weight: 700;
    text-transform: uppercase;
}
.post h2 a {
color:#373b42;
}
.post h2 {
    margin: 0 0 10px;
    padding: 0;
}


.retitle h2 {
    margin: 8px 0;
    display: block;
}
.post-body {
margin: 0px;
padding:10px;
font-size: 14px;
line-height: 26px;
box-sizing:border-box;
text-align:justify;
}

.block-image {
    float: left;
    width: 100%;
    height:auto;
position:relative;
}
.block-image .thumb {
    width: 100%;
    height: auto;
    position: relative;
    display: block;
    overflow: hidden;
}
.block-image .thumb:before {
    background: rgba(0, 0, 0, 0.5);
    bottom: 0px;
    content: "";
    height: 100%;
    width: 100%;
    left: 0px;
    right: 0px;
    margin: 0px auto;
    position: absolute;
opacity:0;
    z-index: 3;
}
.block-image img {
    width: 100%;
    height: 260px;
    display: block;
object-fit:cover;
    transition: all .3s ease-out!important;
    -webkit-transition: all .3s ease-out!important;
    -moz-transition: all .3s ease-out!important;
    -o-transition: all .3s ease-out!important;
}
.block-image:hover .thumb:before {
opacity:1;
}
.date_holder {
    position: absolute;
    top: 10px;
    right: 10px;
    background: $maincolor;
    color: #fff;
    padding: 4px 12px;
}
.date_holder .month {
    display: block;
    text-transform: uppercase;
    font-size: 13px;
    font-weight: 700;
}
.date_holder .day {
    display: block;
    font-size: 20px;
    margin-bottom: 2px;
    font-weight: 700;
}
.post-header {
    padding: 0 10px 10px;
}
.post-meta {
    color: #bdbdbd;
    display: block;
    font-size: 13px;
    font-weight: 400;
    line-height: 21px;
    margin: 0;
    padding: 0;
}
.post-meta a, .post-meta i {
    color: #CBCBCB;
}
.post-timestamp {
    margin-left: 5px;
}
.label-head {
    margin-left: 5px;
}
.label-head a {
    padding-left: 2px;
}
.resumo {
   display:none;
}
.resumo span {
    display: block;
    margin-bottom: 8px;
font-size: 16px;
    line-height: 31px;
}
.post-body img {
max-width: 100%;
padding: 10px 0;
position: relative;
margin:0 auto;
}
.post h3 {
font-size: 18px;
margin-top: 20px;
margin-bottom: 10px;
line-height: 1.1;
}
.second-meta {
    display: none;
}
.comment-link {
    white-space: normal;
}
.ias_trigger {
    clear: both;
    text-align: center;
}
.ias_trigger a {
    padding: 8px;
    color: #fff;
    background: #222;
    border-radius: 4px;
}
.ias_trigger a:hover {
background:$maincolor;
}
#blog-pager {
clear: both;
text-align: center;
padding: 15px 0;
color: #4d4d4d;
}
.home #blog-pager {
display:none;
}
.displaypageNum a,
.showpage a,
.pagecurrent, .blog-pager-older-link, .blog-pager-newer-link {
padding: 5px 13px;
margin-right: 8px;
color: #fff;
background-color: #2b2b2b;
display: inline-block;
line-height: 20px;
-moz-border-radius: 2px;
-webkit-border-radius: 2px;
border-radius: 2px;
margin-top: 10px;
}
.displaypageNum a:hover,
.showpage a:hover,
.pagecurrent, .blog-pager-older-link:hover, .blog-pager-newer-link:hover {
background: $maincolor;
text-decoration: none;
color: #fff;
}
.showpageOf {
display: none!important;
overflow: hidden;
}
#blog-pager .pages {
margin: 10px 0;
border: none;
}
/* ######## Share widget Css ######################### */
.item .post-footer {
padding: 0 10px;
}
.share-box {
position: relative;
padding: 10px 0;
}
.share-title {
border-bottom: 2px solid #777;
color: #010101;
display: inline-block;
padding-bottom: 7px;
font-size: 15px;
font-weight: 500;
position: relative;
top: 2px;
}
.share-art {
float: right;
padding: 0;
padding-top: 0;
font-size: 13px;
font-weight: 400;
text-transform: capitalize;
}
.share-art a {
color: #fff;
padding: 3px 8px;
margin-left: 4px;
border-radius: 2px;
display: inline-block;
margin-right: 0;
background: #010101;
}
.share-art a span {
    display: none;
}
.share-art a:hover{color:#fff}
.share-art .fac-art{background:#3b5998}
.share-art .fac-art:hover{background:rgba(49,77,145,0.7)}
.share-art .twi-art{background:#00acee}
.share-art .twi-art:hover{background:rgba(7,190,237,0.7)}
.share-art .goo-art{background:#db4a39}
.share-art .goo-art:hover{background:rgba(221,75,56,0.7)}
.share-art .pin-art{background:#CA2127}
.share-art .pin-art:hover{background:rgba(202,33,39,0.7)}
.share-art .lin-art{background:#0077B5}
.share-art .lin-art:hover{background:rgba(0,119,181,0.7)}
.share-art .wat-art{background:#25d266;display:none;}
.share-art .wat-art:hover{background:rgba(37, 210, 102, 0.73)}
@media only screen and (max-width: 768px) {
.share-art .wat-art{display:inline-block;}
}
/* ######## Related Post Css ######################### */
#related-posts {
margin-bottom: 10px;
padding: 10px 0;
}
.related li {
width: 32%;
display: inline-block;
height: auto;
min-height: 184px;
float: left;
margin-right: 10px;
overflow: hidden;
position: relative;
}
.related li h3 {
margin-top:0;
}
.related-thumb {
width: 100%;
height: 100px;
overflow: hidden;
border-radius: 2px;
}
.related li .related-img {
width: 100%;
height: 100px;
display: block;
position: relative;
transition: all .3s ease-out!important;
-webkit-transition: all .3s ease-out!important;
-moz-transition: all .3s ease-out!important;
-o-transition: all .3s ease-out!important;
}
.related li .related-img:hover {
-webkit-transform: scale(1.1) rotate(-1.5deg)!important;
-moz-transform: scale(1.1) rotate(-1.5deg)!important;
transform: scale(1.1) rotate(-1.5deg)!important;
transition: all .3s ease-out!important;
-webkit-transition: all .3s ease-out!important;
-moz-transition: all .3s ease-out!important;
-o-transition: all .3s ease-out!important;
}
.related-title a {
font-size: 12px;
line-height: 1.4em;
padding: 10px 0 0;
font-weight: 400;
font-style: normal;
letter-spacing: 1px;
color: #010101;
display: block;
}
.related li:nth-of-type(3n) {
margin-right: 0;
}
.related .related-tag {
display:none;
}
.related-overlay {
position: absolute;
left: 0;
top: 0;
z-index: 1;
width: 100%;
height: 100%;
background-color: rgba(40,35,40,0.05);
}
.related-content {
display: block;
bottom: 0;
padding: 0px 0px 11px;
width: 100%;
line-height: 1.2em;
box-sizing: border-box;
z-index: 2;
}
.related .related-content .recent-date {
font-size: 10px;
}
.recent-date:before, .p-date:before {
content: '\f017';
font-family: fontawesome;
margin-right: 5px;
}
/* ######## Comment Widget Css ######################### */
.comments {
clear: both;
margin: 0;
color: #48494d;
margin-top:10px;
box-sizing: border-box;
border-radius: 5px;
padding: 30px 30px 20px;
background: #FFF;
box-sizing: border-box;
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, .16), 0 2px 10px 0 rgba(0, 0, 0, .12);
}
.post-feeds .feed-links {
display: none;
}
iframe.blogger-iframe-colorize,
iframe.blogger-comment-from-post {
height: 260px!important;
background: #fff;
}
.comment-form {
overflow:hidden;
}
.comments h3 {
line-height:normal;
text-transform:uppercase;
color:#333;
font-weight:bold;
margin:0 0 20px 0;
font-size:14px;
padding:0 0 0 0;
}
h4#comment-post-message {
display:none;
margin:0 0 0 0;
}
.comments h4{
color: #48494d;
border-bottom: 1px solid #efefef;
font-size: 16px;
padding: 12px 0;
margin: 0;
font-weight: 700;
letter-spacing: 1.5px;
text-transform: uppercase;
position: relative;
text-align: left;
}
.comments h4:after {
display: inline-block;
content: "\f075";
font-family: fontAwesome;
font-style: normal;
font-weight: normal;
font-size: 18px;
color: $maincolor;
top: 12px;
right: 15px;
padding: 0;
position: absolute;
}
.comments .comments-content{
font-size:13px;
margin-bottom:8px;
padding: 0;
}
.comments .comments-content .comment-thread ol{
list-style:none;
text-align:left;
margin:13px 0;
padding:0
}
.comments .comments-content .comment-thread ol li{
list-style:none;
}
.comments .avatar-image-container {
background:#fff;
border:1px solid #DDD;
overflow:hidden;
padding:0;
border-radius: 50%;
}
.comments .avatar-image-container img {
border-radius:50%;
}
.comments .comment-block{
position:relative;
background:#fff;
padding:15px;
margin-left:60px;
border: 1px solid #efefef;
}
.comments .comment-block:before {
content:"";
width:0px;
height:0px;
position:absolute;
right:100%;
top:14px;
border-width:10px;
border-style:solid;
border-color:transparent #DDD transparent transparent;
display:block;
}
.comments .comments-content .comment-replies{
margin:8px 0;
margin-left:60px
}
.comments .comments-content .comment-thread:empty{
display:none
}
.comments .comment-replybox-single {
background:#f0f0f0;
padding:0;
margin:8px 0;
margin-left:60px
}
.comments .comment-replybox-thread {
background:#f0f0f0;
margin:8px 0 0 0;
padding:0;
}
.comments .comments-content .comment{
margin-bottom:6px;
padding:0
}
.comments .comments-content .comment:first-child {
padding:0;
margin:0
}
.comments .comments-content .comment:last-child {
padding:0;
margin:0
}
.comments .comment-thread.inline-thread .comment, .comments .comment-thread.inline-thread .comment:last-child {
margin:0px 0px 5px 30%
}
.comment .comment-thread.inline-thread .comment:nth-child(6) {
margin:0px 0px 5px 25%;
}
.comment .comment-thread.inline-thread .comment:nth-child(5) {
margin:0px 0px 5px 20%;
}
.comment .comment-thread.inline-thread .comment:nth-child(4) {
margin:0px 0px 5px 15%;
}
.comment .comment-thread.inline-thread .comment:nth-child(3) {
margin:0px 0px 5px 10%;
}
.comment .comment-thread.inline-thread .comment:nth-child(2) {
margin:0px 0px 5px 5%;
}
.comment .comment-thread.inline-thread .comment:nth-child(1) {
margin:0px 0px 5px 0;
}
.comments .comments-content .comment-thread{
margin:0;
padding:0
}
.comments .comments-content .inline-thread{
background: #fff;
padding:15px;
box-sizing:border-box;
margin:0
}
.comments .comments-content .inline-thread .comment-block {
border-color: $maincolor;
}
.comments .comments-content .inline-thread .comment-block:before {
border-color: transparent $maincolor transparent transparent;
}
.comments .comments-content .user {
letter-spacing: 0.5px;
font-weight: 600;
}
.comments .comments-content .icon.blog-author {
display:inline;
}
.comments .comments-content .icon.blog-author:after {
content: "Author";
background:$maincolor;
color: #fff;
font-size: 11px;
padding: 2px 5px;
text-transform:Capitalize;
font-style:italic;
letter-spacing: 0.3px;
}
.comment-header {
text-transform:uppercase;
font-size:12px;
}
.comments .comments-content .datetime {
margin-left: 6px;
}
.comments .comments-content .datetime a {
color:#888;
}
.comments .comment .comment-actions a {
display:inline-block;
color:#333;
font-weight:bold;
font-size:10px;
line-height:15px;
margin:4px 8px 0 0;
}
.comments .continue a {
color:#333;
display:inline-block;
font-size:10px;
}
.comments .comment .comment-actions a:hover, .comments .continue a:hover{
text-decoration:underline;
}

/* ######## Footer Css ######################### */
.bot-bar-menu {
background-color: $footercolor;
padding: 20px 0px;
overflow: hidden;
}
.bot-menu-wrap {
margin: 0 auto;
position:relative;
text-align:center;
}
.bottom-bar-social {
float:left;
}
.bottom-bar-social li {
display: inline;
padding: 0;
float: left;
margin-right: 5px;
;
}
.bottom-bar-social .widget ul {
padding: 0;
}
.bottom-bar-social .LinkList ul {
text-align: center;
}
.bottom-bar-social #social a {
    display: block;
    font-size: 14px;
    color: #fff;
    padding: 10px 5px;
}
.bottom-bar-social #social a:before {
display: inline-block;
font: normal normal normal 22px/1 FontAwesome;
font-size: inherit;
font-style: normal;
font-weight: 400;
-webkit-font-smoothing: antialiased;
-moz-osx-font-smoothing: grayscale;
}
.bottom-bar-social .bloglovin:before{content:"\f004"}
.bottom-bar-social .facebook:before{content:"\f09a"}
.bottom-bar-social .twitter:before{content:"\f099"}
.bottom-bar-social .gplus:before{content:"\f0d5"}
.bottom-bar-social .rss:before{content:"\f09e"}
.bottom-bar-social .youtube:before{content:"\f167"}
.bottom-bar-social .skype:before{content:"\f17e"}
.bottom-bar-social .stumbleupon:before{content:"\f1a4"}
.bottom-bar-social .tumblr:before{content:"\f173"}
.bottom-bar-social .vine:before{content:"\f1ca"}
.bottom-bar-social .stack-overflow:before{content:"\f16c"}
.bottom-bar-social .linkedin:before{content:"\f0e1"}
.bottom-bar-social .dribbble:before{content:"\f17d"}
.bottom-bar-social .soundcloud:before{content:"\f1be"}
.bottom-bar-social .behance:before{content:"\f1b4"}
.bottom-bar-social .digg:before{content:"\f1a6"}
.bottom-bar-social .instagram:before{content:"\f16d"}
.bottom-bar-social .pinterest:before{content:"\f0d2"}
.bottom-bar-social .delicious:before{content:"\f1a5"}
.bottom-bar-social .codepen:before{content:"\f1cb"}
.bottom-bar-social ul#social a:hover {
color: $maincolor;
opacity: 1;
}
.jugas_footer_copyright {
float:right;
    display: inline-block;
    color: #fff;
line-height:36px;
}
.jugas_footer_copyright a {
color:rgb(246, 77, 77);
}
/* ######## Custom Widget Css ######################### */
.sidebar .FollowByEmail > h3.title,
.sidebar .FollowByEmail .title-wrap {
margin-bottom: 0
}
.FollowByEmail td {
width: 100%;
float: left;
box-sizing: border-box
}
.FollowByEmail .follow-by-email-inner .follow-by-email-submit {
margin-left: 0;
width: 100%;
border-radius: 0;
height: 30px;
font-size: 11px;
color: #fff;
background-color: $maincolor;
font-family: inherit;
text-transform: uppercase;
font-weight: 700;
letter-spacing: 1px
}
.FollowByEmail .follow-by-email-inner .follow-by-email-submit:hover {
opacity:0.8;
}
.FollowByEmail .follow-by-email-inner .follow-by-email-address {
padding-left: 10px;
height: 30px;
border: 1px solid #FFF;
margin-bottom: 5px;
box-sizing: border-box;
font-size: 11px;
font-family: inherit
}
.FollowByEmail .follow-by-email-inner .follow-by-email-address:focus {
border: 1px solid #FFF
}
.FollowByEmail .widget-content {
box-sizing: border-box;
padding: 10px
}
.FollowByEmail .widget-content:before {
content: "Enter your email address to subscribe to this blog and receive notifications of new posts by email.";
font-size: 14px;
color: #f2f2f2;
line-height: 1.4em;
margin-bottom: 5px;
display: block;
padding: 0 2px
}
.item #ads-home {
margin-top: 20px;
}
.cloud-label-widget-content {
display: inline-block;
text-align: left;
}
.cloud-label-widget-content .label-size {
display: inline-block;
float: left;
font-size: 16px;
line-height: normal;
margin: 0 5px 5px 0;
opacity: 1
}
.cloud-label-widget-content .label-size a {
background: #f8f8f8;
color: #878787;
float: left;
font-weight: 400;
line-height: 100%;
margin: 0;
padding: 7px 8px;
text-transform: capitalize;
transition: all .6s;
-webkit-border-radius: 2px;
-moz-border-radius: 2px;
border-radius: 2px;
}
.lowerbar .cloud-label-widget-content .label-size a {
background:#3B3B3B;
}
.cloud-label-widget-content .label-size a:hover,
.cloud-label-widget-content .label-size a:active {
background: $maincolor;
color: #fff;
}
.cloud-label-widget-content .label-size .label-count {
background: $maincolor;
color: #fff;
white-space: nowrap;
display: inline-block;
padding: 6px 8px;
margin-left: -3px;
line-height: normal;
border-radius: 0 2px 2px 0
}
.label-size-1,
.label-size-2 {
opacity: 100
}
.list-label-widget-content li {
display: block;
padding: 8px 0;
position: relative
}
.list-label-widget-content li a:before {
content: '\203a';
position: absolute;
left: 0px;
top: 8px;
font-size: 22px;
color: $maincolor
}
.lowerbar .list-label-widget-content li a {
color:#fff;
}
.list-label-widget-content li a {
color: #0a0a0a;
font-size: 16px;
padding-left: 20px;
font-weight: 400;
text-transform: capitalize;
}
.list-label-widget-content li span:last-child {
color: $maincolor;
font-size: 12px;
font-weight: 700;
position: absolute;
top: 9px;
right: 0
}
.PopularPosts .item-thumbnail {
margin: 0 15px 0 0 !important;
width: 90px;
height: 65px;
float: left;
overflow: hidden;
position: relative
}
.PopularPosts .item-thumbnail a {
position: relative;
display: block;
overflow: hidden;
line-height: 0
}
.PopularPosts ul li img {
width: 90px;
height: 65px;
object-fit: cover;
padding: 0;
transition: all .3s ease
}
.PopularPosts .widget-content ul li {
overflow: hidden;
padding: 10px 0;
border-top: 1px solid #f2f2f2
}
.sidebar .PopularPosts .widget-content ul li:first-child,
.sidebar .custom-widget li:first-child,
.tab-widget .PopularPosts .widget-content ul li:first-child,
.tab-widget .custom-widget li:first-child {
padding-top: 0;
border-top: 0
}
.sidebar .PopularPosts .widget-content ul li:last-child,
.sidebar .custom-widget li:last-child,
.tab-widget .PopularPosts .widget-content ul li:last-child,
.tab-widget .custom-widget li:last-child {
padding-bottom: 0
}
.PopularPosts ul li a {
color: #0a0a0a;
font-weight: 400;
font-size: 13px;
line-height: 1.4em;
transition: color .3s;
}
.PopularPosts ul li a:hover {
color: $maincolor
}
.PopularPosts .item-title {
margin: 0 0 4px;
padding: 0;
line-height: 0
}
.item-snippet {
display: none;
font-size: 0;
padding-top: 0
}
.PopularPosts ul {
counter-reset: popularcount;
margin: 0;
padding: 0;
}
.PopularPosts .item-thumbnail::before {
background: rgba(0, 0, 0, 0.3);
bottom: 0px;
content: "";
height: 100px;
width: 100px;
left: 0px;
right: 0px;
margin: 0px auto;
position: absolute;
z-index: 3;
}
.BlogArchive ul li {
margin-bottom: 7px !important;
padding-bottom: 7px;
}
.BlogArchive ul li:last-child {
margin-bottom: 0;
padding-bottom: 0;
border-bottom: none;
}
.BlogArchive ul li a {
color:#0a0a0a;
}
.BlogArchive ul li a:hover {
color:$maincolor;
}
.BlogArchive .zippy {
color:#e74c3c;
}
.BlogArchive .post-count-link {
font-weight:700;
}
.BlogArchive ul .posts a {
}
.BlogArchive select {
width: 100%;
padding: 10px;
border-color: #777;
}
/* ######## Responsive Css ######################### */
@media only screen and (max-width: 1200px) {
.featured-slider-wrap {
width:auto !important;
}
.sora-author-box-text {
    padding: 30px 70px 0 0;
}
.row {
width: 100%;
float: none;
padding-left: 10px !important;
padding-right: 10px !important;
box-sizing: border-box;
}
.index .post-grid-item, .archive .post-grid-item {
    width: 33.33%;
}
.index .post-grid-item:nth-child(3n), .archive .post-grid-item:nth-child(3n) {
    padding-right: 0;
}
.index .post-grid-item:nth-child(4n), .archive .post-grid-item:nth-child(4n) {
    padding-right: 15px;
}
}
@media only screen and (max-width: 1100px) {
.sora-author-box-text {
    padding: 15px 0 0 0;
}
.sora-author-box img {
    margin-right: 40px;
max-width: 400px;
}
div#sora_blogger_cntct_form .wrap-me {
    max-width: 500px;
    float: none;
    clear: both;
    margin: 0 auto 20px;
    width: 100%;
}
.map-me {
    max-width: 500px;
    float: none;
    clear: both;
    margin: 0 auto;
    width: 100%;
}
}
@media only screen and (max-width: 980px) {

.item #main-wrapper, .statc_page #main-wrapper, .item #sidebar-wrapper, .statc_page #sidebar-wrapper {
float: none;
clear: both;
width: 100%;
margin: 0 auto;
}
#main-wrapper {
max-width: 100%;
}
#sidebar-wrapper {
padding-top: 20px;
}
#nav1, #nav {
display: none;
}
.slicknav_menu {
    display: block;
}
.item .tm-menu .slicknav_menu, .static_page .tm-menu .slicknav_menu, .error_page {
display:block;
}
.tm-menu, #menu {
height: auto;
}
.item .tm-menu, .static_page .tm-menu, .error_page .tm-menu {
float:none;
display:block;
}
}
@media screen and (max-width: 940px) {
.background-container {
    display: none;
}
.hero-row {
    width: 100%;
}
.fenix-sub-head {
    margin-top: 0;
}
.skill-wrapper .skill-progress {
    max-width: 120px;
    width: 100%;
    margin: 0;
}
}
@media screen and (max-width: 880px) {
.sora-author-box {
    padding: 20px 10px;
}
.home #header-wrapper {
margin-bottom: 10px;
}
.item #content-wrapper {
padding: 10px 0 30px;
}
.skills, .skill-details {
    width: 100%;
    float: none;
    padding: 20px;
    clear: both;
}
}
@media only screen and (max-width: 768px) {
.sora-author-box img {
    margin-right: 0;
    max-width: 100%;
    float: none;
    width: 100%;
    height: auto;
    clear: both;
}
.sora-author-box-text {
    padding: 10px;
    text-align: center;
}
.counter-box-item, .works-tiles {
    width: 50%;
}

#header h1 {
    font-size: 50px;
}
.index .post-grid-item:nth-child(3n), .archive .post-grid-item:nth-child(3n) {
   padding-right: 0;
}
.index .post-grid-item:nth-child(4n), .archive .post-grid-item:nth-child(4n) {
   padding-right: 0;
}
.index .post-grid-item, .archive .post-grid-item {
    width: 100%;
padding-right: 0;
}
.tm-menu {
    text-align: center;
}
.top-bar-social {
    float: none;
    width: 100%;
    clear: both;
    overflow: hidden;
}
.top-bar-social li {
    display: inline-block;
    float: none;
}
.flickity-prev-next-button {
display:none;
}
.bot-menu, .bottom-bar-social {
    float: none;
    width: 100%;
    clear: both;
    overflow: hidden;
    position: static;
}
.bot-menu ul {
text-align:center;
}
.bot-menu ul li {
    float: none;
}
.bottom-bar-social li {
    float: none;
    display: inline-block;
}
.related li {
    width: 31%;
}
.jugas_footer_copyright {
    float: none;
}
.share-art span {
display: none;
}
.ops-404 {
width: 80%!important;
}
.title-404 {
font-size: 160px!important;
}
#header {
padding: 10px 0px 0;
}
}
@media only screen and (max-width: 767px) {
#header {
    padding: 0;
}
.sora-author-box {
    padding: 10px;
}
#header h1 {
    font-size: 30px;
}
.header-text p {
    font-size: 30px;
}
.sora-author-box-image {
    width: 100%;
    float: none;
    margin-right: 0;
    margin-bottom: 10px;
}
.slide-in {
display:none;
}
.entry {
    width: 100%;
    box-sizing: border-box;
}
.entry:after, .timeline:after {
display:none;
}
.entry--right {
    margin-left: 0;
}
.sora-cv-hobby-details .card-action ul li span {
    display: none;
}
.price_card {
    width: 100%;
    padding-right: 0;
    margin-bottom: 10px;
    float: none;
    clear: both;
}
.price_card:not(:last-child) {
    padding-right: 0;
}
.sora-cv-author-details .card-content {
    padding: 10px;
}
.sora-cv-author-details .card-action {
    padding: 10px;
}
.entry {
    padding: 10px;
}
}
@media only screen and (max-width: 480px) {
.skill-wrapper .skill-progress {
    margin-bottom: 30px;
}
.comments .comments-content .comment-replies {
    margin-left: 0;
}
.special-title h4, .works-title h4, .sora-cv-hobby-details .hobby-title h4, .Portfolio-title h4, .testimonial-title h4, .about-title h4, .contact-title h4 {
    font-size: 18px;
}
.sora-cv-hobby-details .card-action ul li {
    width: 33.33%;
    padding: 15px;
}
.sora-cv-hobby-details .card-action ul li i {
    font-size: 16px;
}
.slide-in {
display:block;
}
.special-tiles, .works-tiles, .about-tiles, .counter-box-item {
    width: 100%;
}

#header h1 {
    font-size: 30px;
}
.header-text p {
    font-size: 20px;
}
.header-logo-desc span, .header-logo-desc p {
    font-size: 16px;
}
.index .post h2,.archive .post h2, .sora-slide .ty-bonos-entry a, #first-post .post h2 {
line-height: 34px;
font-size: 23px;
}
h1.post-title {
font-size: 22px;
margin-bottom: 10px;
}
#sidebar-wrapper {
max-width: 100%;
}
.share-title {
    display: none;
}
.share-art {
    float: none;
    text-align: center;
}
.related li {
width: 100%;
margin:0 auto;
}
.index .post-outer {
padding: 0 0 5x;
}
}
@media only screen and (max-width: 360px) {
.title-404 {
font-size: 150px!important;
}
.header-logo-desc p {
    font-size: 100%;
}
#header h1 {
    font-size: 250%;
}
}
@media only screen and (max-width: 300px) {
#sidebar-wrapper, .feat-slider-wrap {display:none}
.archive .post h2,.index .post h2, #first-post .post h2 {
line-height: 29px!important;
font-size: 15px!important;
}
article {
overflow: hidden;
}
#blog-pager {
padding: 0;
margin: 0;
}
.index .snippets,.archive .snippets {
display: none;
}
.share-art, .share-box .post-author {
float: none !important;
margin: 0 auto;
text-align: center;
clear: both;
}
.read-more-wrap, .post-labels {
float: none !important;
clear: both;
display: block;
text-align: center;
}
.ops-404 {
font-size: 20px!important;
}
.title-404 {
font-size: 120px!important;
}
h1.post-title {
font-size: 17px;
}
.share-box {
overflow: hidden;
}
.top-bar-social #social a {
width: 24px;
height: 24px;
line-height: 24px;
}
.second-meta .share-art a {
padding: 5px;
}
.comments .avatar-image-container {
display: none;
}
.comments .comment-block {
margin-left: 0 !important;
position: relative;
}
}
]]></b:skin>
<b:if cond='data:blog.url == data:blog.homepageUrl'>
<style>

/*!
 * animate.css -http://daneden.me/animate
 * Version - 3.5.2
 * Licensed under the MIT license - http://opensource.org/licenses/MIT
 *
 * Copyright (c) 2017 Daniel Eden
 */

.animated{animation-duration:1s;animation-fill-mode:both}.animated.infinite{animation-iteration-count:infinite}.animated.hinge{animation-duration:2s}.animated.bounceIn,.animated.bounceOut,.animated.flipOutX,.animated.flipOutY{animation-duration:.75s}@keyframes bounce{0%,20%,53%,80%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1);transform:translateZ(0)}40%,43%{animation-timing-function:cubic-bezier(.755,.05,.855,.06);transform:translate3d(0,-30px,0)}70%{animation-timing-function:cubic-bezier(.755,.05,.855,.06);transform:translate3d(0,-15px,0)}90%{transform:translate3d(0,-4px,0)}}.bounce{animation-name:bounce;transform-origin:center bottom}@keyframes flash{0%,50%,to{opacity:1}25%,75%{opacity:0}}.flash{animation-name:flash}@keyframes pulse{0%{transform:scaleX(1)}50%{transform:scale3d(1.05,1.05,1.05)}to{transform:scaleX(1)}}.pulse{animation-name:pulse}@keyframes rubberBand{0%{transform:scaleX(1)}30%{transform:scale3d(1.25,.75,1)}40%{transform:scale3d(.75,1.25,1)}50%{transform:scale3d(1.15,.85,1)}65%{transform:scale3d(.95,1.05,1)}75%{transform:scale3d(1.05,.95,1)}to{transform:scaleX(1)}}.rubberBand{animation-name:rubberBand}@keyframes shake{0%,to{transform:translateZ(0)}10%,30%,50%,70%,90%{transform:translate3d(-10px,0,0)}20%,40%,60%,80%{transform:translate3d(10px,0,0)}}.shake{animation-name:shake}@keyframes headShake{0%{transform:translateX(0)}6.5%{transform:translateX(-6px) rotateY(-9deg)}18.5%{transform:translateX(5px) rotateY(7deg)}31.5%{transform:translateX(-3px) rotateY(-5deg)}43.5%{transform:translateX(2px) rotateY(3deg)}50%{transform:translateX(0)}}.headShake{animation-timing-function:ease-in-out;animation-name:headShake}@keyframes swing{20%{transform:rotate(15deg)}40%{transform:rotate(-10deg)}60%{transform:rotate(5deg)}80%{transform:rotate(-5deg)}to{transform:rotate(0deg)}}.swing{transform-origin:top center;animation-name:swing}@keyframes tada{0%{transform:scaleX(1)}10%,20%{transform:scale3d(.9,.9,.9) rotate(-3deg)}30%,50%,70%,90%{transform:scale3d(1.1,1.1,1.1) rotate(3deg)}40%,60%,80%{transform:scale3d(1.1,1.1,1.1) rotate(-3deg)}to{transform:scaleX(1)}}.tada{animation-name:tada}@keyframes wobble{0%{transform:none}15%{transform:translate3d(-25%,0,0) rotate(-5deg)}30%{transform:translate3d(20%,0,0) rotate(3deg)}45%{transform:translate3d(-15%,0,0) rotate(-3deg)}60%{transform:translate3d(10%,0,0) rotate(2deg)}75%{transform:translate3d(-5%,0,0) rotate(-1deg)}to{transform:none}}.wobble{animation-name:wobble}@keyframes jello{0%,11.1%,to{transform:none}22.2%{transform:skewX(-12.5deg) skewY(-12.5deg)}33.3%{transform:skewX(6.25deg) skewY(6.25deg)}44.4%{transform:skewX(-3.125deg) skewY(-3.125deg)}55.5%{transform:skewX(1.5625deg) skewY(1.5625deg)}66.6%{transform:skewX(-.78125deg) skewY(-.78125deg)}77.7%{transform:skewX(.390625deg) skewY(.390625deg)}88.8%{transform:skewX(-.1953125deg) skewY(-.1953125deg)}}.jello{animation-name:jello;transform-origin:center}@keyframes bounceIn{0%,20%,40%,60%,80%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:scale3d(.3,.3,.3)}20%{transform:scale3d(1.1,1.1,1.1)}40%{transform:scale3d(.9,.9,.9)}60%{opacity:1;transform:scale3d(1.03,1.03,1.03)}80%{transform:scale3d(.97,.97,.97)}to{opacity:1;transform:scaleX(1)}}.bounceIn{animation-name:bounceIn}@keyframes bounceInDown{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,-3000px,0)}60%{opacity:1;transform:translate3d(0,25px,0)}75%{transform:translate3d(0,-10px,0)}90%{transform:translate3d(0,5px,0)}to{transform:none}}.bounceInDown{animation-name:bounceInDown}@keyframes bounceInLeft{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(-3000px,0,0)}60%{opacity:1;transform:translate3d(25px,0,0)}75%{transform:translate3d(-10px,0,0)}90%{transform:translate3d(5px,0,0)}to{transform:none}}.bounceInLeft{animation-name:bounceInLeft}@keyframes bounceInRight{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(3000px,0,0)}60%{opacity:1;transform:translate3d(-25px,0,0)}75%{transform:translate3d(10px,0,0)}90%{transform:translate3d(-5px,0,0)}to{transform:none}}.bounceInRight{animation-name:bounceInRight}@keyframes bounceInUp{0%,60%,75%,90%,to{animation-timing-function:cubic-bezier(.215,.61,.355,1)}0%{opacity:0;transform:translate3d(0,3000px,0)}60%{opacity:1;transform:translate3d(0,-20px,0)}75%{transform:translate3d(0,10px,0)}90%{transform:translate3d(0,-5px,0)}to{transform:translateZ(0)}}.bounceInUp{animation-name:bounceInUp}@keyframes bounceOut{20%{transform:scale3d(.9,.9,.9)}50%,55%{opacity:1;transform:scale3d(1.1,1.1,1.1)}to{opacity:0;transform:scale3d(.3,.3,.3)}}.bounceOut{animation-name:bounceOut}@keyframes bounceOutDown{20%{transform:translate3d(0,10px,0)}40%,45%{opacity:1;transform:translate3d(0,-20px,0)}to{opacity:0;transform:translate3d(0,2000px,0)}}.bounceOutDown{animation-name:bounceOutDown}@keyframes bounceOutLeft{20%{opacity:1;transform:translate3d(20px,0,0)}to{opacity:0;transform:translate3d(-2000px,0,0)}}.bounceOutLeft{animation-name:bounceOutLeft}@keyframes bounceOutRight{20%{opacity:1;transform:translate3d(-20px,0,0)}to{opacity:0;transform:translate3d(2000px,0,0)}}.bounceOutRight{animation-name:bounceOutRight}@keyframes bounceOutUp{20%{transform:translate3d(0,-10px,0)}40%,45%{opacity:1;transform:translate3d(0,20px,0)}to{opacity:0;transform:translate3d(0,-2000px,0)}}.bounceOutUp{animation-name:bounceOutUp}@keyframes fadeIn{0%{opacity:0}to{opacity:1}}.fadeIn{animation-name:fadeIn}@keyframes fadeInDown{0%{opacity:0;transform:translate3d(0,-100%,0)}to{opacity:1;transform:none}}.fadeInDown{animation-name:fadeInDown}@keyframes fadeInDownBig{0%{opacity:0;transform:translate3d(0,-2000px,0)}to{opacity:1;transform:none}}.fadeInDownBig{animation-name:fadeInDownBig}@keyframes fadeInLeft{0%{opacity:0;transform:translate3d(-100%,0,0)}to{opacity:1;transform:none}}.fadeInLeft{animation-name:fadeInLeft}@keyframes fadeInLeftBig{0%{opacity:0;transform:translate3d(-2000px,0,0)}to{opacity:1;transform:none}}.fadeInLeftBig{animation-name:fadeInLeftBig}@keyframes fadeInRight{0%{opacity:0;transform:translate3d(100%,0,0)}to{opacity:1;transform:none}}.fadeInRight{animation-name:fadeInRight}@keyframes fadeInRightBig{0%{opacity:0;transform:translate3d(2000px,0,0)}to{opacity:1;transform:none}}.fadeInRightBig{animation-name:fadeInRightBig}@keyframes fadeInUp{0%{opacity:0;transform:translate3d(0,100%,0)}to{opacity:1;transform:none}}.fadeInUp{animation-name:fadeInUp}@keyframes fadeInUpBig{0%{opacity:0;transform:translate3d(0,2000px,0)}to{opacity:1;transform:none}}.fadeInUpBig{animation-name:fadeInUpBig}@keyframes fadeOut{0%{opacity:1}to{opacity:0}}.fadeOut{animation-name:fadeOut}@keyframes fadeOutDown{0%{opacity:1}to{opacity:0;transform:translate3d(0,100%,0)}}.fadeOutDown{animation-name:fadeOutDown}@keyframes fadeOutDownBig{0%{opacity:1}to{opacity:0;transform:translate3d(0,2000px,0)}}.fadeOutDownBig{animation-name:fadeOutDownBig}@keyframes fadeOutLeft{0%{opacity:1}to{opacity:0;transform:translate3d(-100%,0,0)}}.fadeOutLeft{animation-name:fadeOutLeft}@keyframes fadeOutLeftBig{0%{opacity:1}to{opacity:0;transform:translate3d(-2000px,0,0)}}.fadeOutLeftBig{animation-name:fadeOutLeftBig}@keyframes fadeOutRight{0%{opacity:1}to{opacity:0;transform:translate3d(100%,0,0)}}.fadeOutRight{animation-name:fadeOutRight}@keyframes fadeOutRightBig{0%{opacity:1}to{opacity:0;transform:translate3d(2000px,0,0)}}.fadeOutRightBig{animation-name:fadeOutRightBig}@keyframes fadeOutUp{0%{opacity:1}to{opacity:0;transform:translate3d(0,-100%,0)}}.fadeOutUp{animation-name:fadeOutUp}@keyframes fadeOutUpBig{0%{opacity:1}to{opacity:0;transform:translate3d(0,-2000px,0)}}.fadeOutUpBig{animation-name:fadeOutUpBig}@keyframes flip{0%{transform:perspective(400px) rotateY(-1turn);animation-timing-function:ease-out}40%{transform:perspective(400px) translateZ(150px) rotateY(-190deg);animation-timing-function:ease-out}50%{transform:perspective(400px) translateZ(150px) rotateY(-170deg);animation-timing-function:ease-in}80%{transform:perspective(400px) scale3d(.95,.95,.95);animation-timing-function:ease-in}to{transform:perspective(400px);animation-timing-function:ease-in}}.animated.flip{-webkit-backface-visibility:visible;backface-visibility:visible;animation-name:flip}@keyframes flipInX{0%{transform:perspective(400px) rotateX(90deg);animation-timing-function:ease-in;opacity:0}40%{transform:perspective(400px) rotateX(-20deg);animation-timing-function:ease-in}60%{transform:perspective(400px) rotateX(10deg);opacity:1}80%{transform:perspective(400px) rotateX(-5deg)}to{transform:perspective(400px)}}.flipInX{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;animation-name:flipInX}@keyframes flipInY{0%{transform:perspective(400px) rotateY(90deg);animation-timing-function:ease-in;opacity:0}40%{transform:perspective(400px) rotateY(-20deg);animation-timing-function:ease-in}60%{transform:perspective(400px) rotateY(10deg);opacity:1}80%{transform:perspective(400px) rotateY(-5deg)}to{transform:perspective(400px)}}.flipInY{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;animation-name:flipInY}@keyframes flipOutX{0%{transform:perspective(400px)}30%{transform:perspective(400px) rotateX(-20deg);opacity:1}to{transform:perspective(400px) rotateX(90deg);opacity:0}}.flipOutX{animation-name:flipOutX;-webkit-backface-visibility:visible!important;backface-visibility:visible!important}@keyframes flipOutY{0%{transform:perspective(400px)}30%{transform:perspective(400px) rotateY(-15deg);opacity:1}to{transform:perspective(400px) rotateY(90deg);opacity:0}}.flipOutY{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;animation-name:flipOutY}@keyframes lightSpeedIn{0%{transform:translate3d(100%,0,0) skewX(-30deg);opacity:0}60%{transform:skewX(20deg);opacity:1}80%{transform:skewX(-5deg);opacity:1}to{transform:none;opacity:1}}.lightSpeedIn{animation-name:lightSpeedIn;animation-timing-function:ease-out}@keyframes lightSpeedOut{0%{opacity:1}to{transform:translate3d(100%,0,0) skewX(30deg);opacity:0}}.lightSpeedOut{animation-name:lightSpeedOut;animation-timing-function:ease-in}@keyframes rotateIn{0%{transform-origin:center;transform:rotate(-200deg);opacity:0}to{transform-origin:center;transform:none;opacity:1}}.rotateIn{animation-name:rotateIn}@keyframes rotateInDownLeft{0%{transform-origin:left bottom;transform:rotate(-45deg);opacity:0}to{transform-origin:left bottom;transform:none;opacity:1}}.rotateInDownLeft{animation-name:rotateInDownLeft}@keyframes rotateInDownRight{0%{transform-origin:right bottom;transform:rotate(45deg);opacity:0}to{transform-origin:right bottom;transform:none;opacity:1}}.rotateInDownRight{animation-name:rotateInDownRight}@keyframes rotateInUpLeft{0%{transform-origin:left bottom;transform:rotate(45deg);opacity:0}to{transform-origin:left bottom;transform:none;opacity:1}}.rotateInUpLeft{animation-name:rotateInUpLeft}@keyframes rotateInUpRight{0%{transform-origin:right bottom;transform:rotate(-90deg);opacity:0}to{transform-origin:right bottom;transform:none;opacity:1}}.rotateInUpRight{animation-name:rotateInUpRight}@keyframes rotateOut{0%{transform-origin:center;opacity:1}to{transform-origin:center;transform:rotate(200deg);opacity:0}}.rotateOut{animation-name:rotateOut}@keyframes rotateOutDownLeft{0%{transform-origin:left bottom;opacity:1}to{transform-origin:left bottom;transform:rotate(45deg);opacity:0}}.rotateOutDownLeft{animation-name:rotateOutDownLeft}@keyframes rotateOutDownRight{0%{transform-origin:right bottom;opacity:1}to{transform-origin:right bottom;transform:rotate(-45deg);opacity:0}}.rotateOutDownRight{animation-name:rotateOutDownRight}@keyframes rotateOutUpLeft{0%{transform-origin:left bottom;opacity:1}to{transform-origin:left bottom;transform:rotate(-45deg);opacity:0}}.rotateOutUpLeft{animation-name:rotateOutUpLeft}@keyframes rotateOutUpRight{0%{transform-origin:right bottom;opacity:1}to{transform-origin:right bottom;transform:rotate(90deg);opacity:0}}.rotateOutUpRight{animation-name:rotateOutUpRight}@keyframes hinge{0%{transform-origin:top left;animation-timing-function:ease-in-out}20%,60%{transform:rotate(80deg);transform-origin:top left;animation-timing-function:ease-in-out}40%,80%{transform:rotate(60deg);transform-origin:top left;animation-timing-function:ease-in-out;opacity:1}to{transform:translate3d(0,700px,0);opacity:0}}.hinge{animation-name:hinge}@keyframes jackInTheBox{0%{opacity:0;transform:scale(.1) rotate(30deg);transform-origin:center bottom}50%{transform:rotate(-10deg)}70%{transform:rotate(3deg)}to{opacity:1;transform:scale(1)}}.jackInTheBox{animation-name:jackInTheBox}@keyframes rollIn{0%{opacity:0;transform:translate3d(-100%,0,0) rotate(-120deg)}to{opacity:1;transform:none}}.rollIn{animation-name:rollIn}@keyframes rollOut{0%{opacity:1}to{opacity:0;transform:translate3d(100%,0,0) rotate(120deg)}}.rollOut{animation-name:rollOut}@keyframes zoomIn{0%{opacity:0;transform:scale3d(.3,.3,.3)}50%{opacity:1}}.zoomIn{animation-name:zoomIn}@keyframes zoomInDown{0%{opacity:0;transform:scale3d(.1,.1,.1) translate3d(0,-1000px,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}60%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(0,60px,0);animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomInDown{animation-name:zoomInDown}@keyframes zoomInLeft{0%{opacity:0;transform:scale3d(.1,.1,.1) translate3d(-1000px,0,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}60%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(10px,0,0);animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomInLeft{animation-name:zoomInLeft}@keyframes zoomInRight{0%{opacity:0;transform:scale3d(.1,.1,.1) translate3d(1000px,0,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}60%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(-10px,0,0);animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomInRight{animation-name:zoomInRight}@keyframes zoomInUp{0%{opacity:0;transform:scale3d(.1,.1,.1) translate3d(0,1000px,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}60%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomInUp{animation-name:zoomInUp}@keyframes zoomOut{0%{opacity:1}50%{opacity:0;transform:scale3d(.3,.3,.3)}to{opacity:0}}.zoomOut{animation-name:zoomOut}@keyframes zoomOutDown{40%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}to{opacity:0;transform:scale3d(.1,.1,.1) translate3d(0,2000px,0);transform-origin:center bottom;animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomOutDown{animation-name:zoomOutDown}@keyframes zoomOutLeft{40%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(42px,0,0)}to{opacity:0;transform:scale(.1) translate3d(-2000px,0,0);transform-origin:left center}}.zoomOutLeft{animation-name:zoomOutLeft}@keyframes zoomOutRight{40%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(-42px,0,0)}to{opacity:0;transform:scale(.1) translate3d(2000px,0,0);transform-origin:right center}}.zoomOutRight{animation-name:zoomOutRight}@keyframes zoomOutUp{40%{opacity:1;transform:scale3d(.475,.475,.475) translate3d(0,60px,0);animation-timing-function:cubic-bezier(.55,.055,.675,.19)}to{opacity:0;transform:scale3d(.1,.1,.1) translate3d(0,-2000px,0);transform-origin:center bottom;animation-timing-function:cubic-bezier(.175,.885,.32,1)}}.zoomOutUp{animation-name:zoomOutUp}@keyframes slideInDown{0%{transform:translate3d(0,-100%,0);visibility:visible}to{transform:translateZ(0)}}.slideInDown{animation-name:slideInDown}@keyframes slideInLeft{0%{transform:translate3d(-100%,0,0);visibility:visible}to{transform:translateZ(0)}}.slideInLeft{animation-name:slideInLeft}@keyframes slideInRight{0%{transform:translate3d(100%,0,0);visibility:visible}to{transform:translateZ(0)}}.slideInRight{animation-name:slideInRight}@keyframes slideInUp{0%{transform:translate3d(0,100%,0);visibility:visible}to{transform:translateZ(0)}}.slideInUp{animation-name:slideInUp}@keyframes slideOutDown{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,100%,0)}}.slideOutDown{animation-name:slideOutDown}@keyframes slideOutLeft{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(-100%,0,0)}}.slideOutLeft{animation-name:slideOutLeft}@keyframes slideOutRight{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(100%,0,0)}}.slideOutRight{animation-name:slideOutRight}@keyframes slideOutUp{0%{transform:translateZ(0)}to{visibility:hidden;transform:translate3d(0,-100%,0)}}.slideOutUp{animation-name:slideOutUp}
</style>
    </b:if>
<style>
/*-------Typography and ShortCodes-------*/
.firstcharacter{float:left;color:#27ae60;font-size:75px;line-height:60px;padding-top:4px;padding-right:8px;padding-left:3px}.post-body h1,.post-body h2,.post-body h3,.post-body h4,.post-body h5,.post-body h6{margin-bottom:15px;color:#2c3e50}blockquote{font-style:italic;color:#888;border-left:5px solid #27ae60;margin-left:0;padding:10px 15px}blockquote:before{content:&#39;\f10d&#39;;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;margin-right:10px;color:#888}blockquote:after{content:&#39;\f10e&#39;;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;margin-left:10px;color:#888}.button{background-color:#2c3e50;float:left;padding:5px 12px;margin:5px;color:#fff;text-align:center;border:0;cursor:pointer;border-radius:3px;display:block;text-decoration:none;font-weight:400;transition:all .3s ease-out !important;-webkit-transition:all .3s ease-out !important}a.button{color:#fff}.button:hover{background-color:#27ae60;color:#fff}.button.small{font-size:12px;padding:5px 12px}.button.medium{font-size:16px;padding:6px 15px}.button.large{font-size:18px;padding:8px 18px}.small-button{width:100%;overflow:hidden;clear:both}.medium-button{width:100%;overflow:hidden;clear:both}.large-button{width:100%;overflow:hidden;clear:both}.demo:before{content:&quot;\f06e&quot;;margin-right:5px;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:normal;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.download:before{content:&quot;\f019&quot;;margin-right:5px;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:normal;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.buy:before{content:&quot;\f09d&quot;;margin-right:5px;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:normal;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.visit:before{content:&quot;\f14c&quot;;margin-right:5px;display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:400;line-height:normal;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.widget .post-body ul,.widget .post-body ol{line-height:1.5;font-weight:400}.widget .post-body li{margin:5px 0;padding:0;line-height:1.5}.post-body ul li:before{content:&quot;\f105&quot;;margin-right:5px;font-family:fontawesome}pre{font-family:Monaco, &quot;Andale Mono&quot;, &quot;Courier New&quot;, Courier, monospace;background-color:#2c3e50;background-image:-webkit-linear-gradient(rgba(0, 0, 0, 0.05) 50%, transparent 50%, transparent);background-image:-moz-linear-gradient(rgba(0, 0, 0, 0.05) 50%, transparent 50%, transparent);background-image:-ms-linear-gradient(rgba(0, 0, 0, 0.05) 50%, transparent 50%, transparent);background-image:-o-linear-gradient(rgba(0, 0, 0, 0.05) 50%, transparent 50%, transparent);background-image:linear-gradient(rgba(0, 0, 0, 0.05) 50%, transparent 50%, transparent);-webkit-background-size:100% 50px;-moz-background-size:100% 50px;background-size:100% 50px;line-height:25px;color:#f1f1f1;position:relative;padding:0 7px;margin:15px 0 10px;overflow:hidden;word-wrap:normal;white-space:pre;position:relative}pre:before{content:&#39;Code&#39;;display:block;background:#F7F7F7;margin-left:-7px;margin-right:-7px;color:#2c3e50;padding-left:7px;font-weight:400;font-size:14px}pre code,pre .line-number{display:block}pre .line-number a{color:#27ae60;opacity:0.6}pre .line-number span{display:block;float:left;clear:both;width:20px;text-align:center;margin-left:-7px;margin-right:7px}pre .line-number span:nth-child(odd){background-color:rgba(0, 0, 0, 0.11)}pre .line-number span:nth-child(even){background-color:rgba(255, 255, 255, 0.05)}pre .cl{display:block;clear:both}#contact{background-color:#fff;margin:30px 0 !important}#contact .contact-form-widget{max-width:100% !important}#contact .contact-form-name,#contact .contact-form-email,#contact .contact-form-email-message{background-color:#FFF;border:1px solid #eee;border-radius:3px;padding:10px;margin-bottom:10px !important;max-width:100% !important}#contact .contact-form-name{width:47.7%;height:50px}#contact .contact-form-email{width:49.7%;height:50px}#contact .contact-form-email-message{height:150px}#contact .contact-form-button-submit{max-width:100%;width:100%;z-index:0;margin:4px 0 0;padding:10px !important;text-align:center;cursor:pointer;background:#27ae60;border:0;height:auto;-webkit-border-radius:2px;-moz-border-radius:2px;-ms-border-radius:2px;-o-border-radius:2px;border-radius:2px;text-transform:uppercase;-webkit-transition:all .2s ease-out;-moz-transition:all .2s ease-out;-o-transition:all .2s ease-out;-ms-transition:all .2s ease-out;transition:all .2s ease-out;color:#FFF}#contact .contact-form-button-submit:hover{background:#2c3e50}#contact .contact-form-email:focus,#contact .contact-form-name:focus,#contact .contact-form-email-message:focus{box-shadow:none !important}.alert-message{position:relative;display:block;background-color:#FAFAFA;padding:20px;margin:20px 0;-webkit-border-radius:2px;-moz-border-radius:2px;border-radius:2px;color:#2f3239;border:1px solid}.alert-message p{margin:0 !important;padding:0;line-height:22px;font-size:13px;color:#2f3239}.alert-message span{font-size:14px !important}.alert-message i{font-size:16px;line-height:20px}.alert-message.success{background-color:#f1f9f7;border-color:#e0f1e9;color:#1d9d74}.alert-message.success a,.alert-message.success span{color:#1d9d74}.alert-message.alert{background-color:#DAEFFF;border-color:#8ED2FF;color:#378FFF}.alert-message.alert a,.alert-message.alert span{color:#378FFF}.alert-message.warning{background-color:#fcf8e3;border-color:#faebcc;color:#8a6d3b}.alert-message.warning a,.alert-message.warning span{color:#8a6d3b}.alert-message.error{background-color:#FFD7D2;border-color:#FF9494;color:#F55D5D}.alert-message.error a,.alert-message.error span{color:#F55D5D}.fa-check-circle:before{content:&quot;\f058&quot;}.fa-info-circle:before{content:&quot;\f05a&quot;}.fa-exclamation-triangle:before{content:&quot;\f071&quot;}.fa-exclamation-circle:before{content:&quot;\f06a&quot;}.post-table table{border-collapse:collapse;width:100%}.post-table th{background-color:#eee;font-weight:bold}.post-table th,.post-table td{border:0.125em solid #333;line-height:1.5;padding:0.75em;text-align:left}@media (max-width: 30em){.post-table thead tr{position:absolute;top:-9999em;left:-9999em}.post-table tr{border:0.125em solid #333;border-bottom:0}.post-table tr + tr{margin-top:1.5em}.post-table tr,.post-table td{display:block}.post-table td{border:none;border-bottom:0.125em solid #333;padding-left:50%}.post-table td:before{content:attr(data-label);display:inline-block;font-weight:bold;line-height:1.5;margin-left:-100%;width:100%}}@media (max-width: 20em){.post-table td{padding-left:0.75em}.post-table td:before{display:block;margin-bottom:0.75em;margin-left:0}}
.FollowByEmail {
    clear: both;
}
</style>

<b:template-skin><![CDATA[
/*------Layout (No Edit)----------*/
#layout #preloader, #layout .scrolling-menu {
    display: none;
}
#layout .sora-contact-widget {
display:none;
}
body#layout .sora-author-box, body#layout .sora-cv-hobby-details {
    display: none;
}
body#layout #outer-wrapper {
padding: 0;
width: 800px
}
body#layout .section h4 {
color: #333!important;
text-align:center;
text-transform:uppercase;
letter-spacing:1.5px;
}

body#layout .tm-menu, body#layout #menu {
height: auto;
position:static;
}
body#layout #menu .widget {
display: block;
visibility:visible;
}
body#layout #header-wrapper {
    height: auto;
}
body#layout #content-wrapper {
margin: 0 auto;
padding:0;
}
body#layout #main-wrapper {
float: left;
width: 70%;
margin: 0;
padding: 0
}
body#layout #sidebar-wrapper {
float: right;
width: 30%;
margin: 0;
padding: 0;
    display: block;
    visibility: visible;
    height: auto;
    opacity: 1;
}
body#layout #sidebar-wrapper .section {
background-color: #f8e244 !important;
border: 1px solid #fff
}
body#layout #sidebar-wrapper .section h4 {
color:#fff;
}
body#layout #sidebar-wrapper .section .widget-content {
border-color: #5a7ea2!important
}
body#layout #sidebar-wrapper .section .draggable-widget .widget-wrap2 {
background-color: #0080ce !important
}
body#layout #main-wrapper #main {
margin-right: 4px;
background-color: #5a7ea2;
border-color: #34495e
}
body#layout #main-wrapper #main h4 {
color: #fff!important
}
body#layout .layout-widget-description {
display: none!important
}
body#layout #Blog1 .widget-content {
border-color: #34495e
}
body#layout .draggable-widget .widget-wrap2 {
background: #0080ce url(https://www.blogger.com/img/widgets/draggable.png) no-repeat 4px 50%;
}
body#layout .editlink {
background: #0080ce;
color: #fff !important;
padding: 0 3px;
line-height: 18px;
border: 1px solid #2469d9;
border-radius: 3px;
text-transform: uppercase;
letter-spacing: 1px;
text-decoration: none !important;
}
body#layout .add_widget {
background: #fff;
}
body#layout .tm-menu .section {
background-color: #f6b3d2 !important;
border: 1px solid #ed67a7
}
body#layout .header {
background-color: #f2132d !important;
border: 1px solid #f53551
}
body#layout .feat-slider-wrap .section {
background-color: #a0d3db !important;
border: 1px solid #a2dbeb
}
body#layout .insta-wrap .section {
background-color: #a0d3db !important;
border: 1px solid #a2dbeb
}
body#layout .FollowByEmail .widget-content:before, body#layout .jugas_footer_copyright {
display:none;
}

body#layout .sora-special-box, body#layout .sora-works-box, body#layout .sora-about-box, body#layout .insta-wrap, body#layout  .Portfolio-title {display:none;}
/*------Layout (end)----------*/
]]></b:template-skin>

<b:include data='blog' name='google-analytics'/>
<script type='text/javascript'> 
//<![CDATA[
var no_image = "http://3.bp.blogspot.com/-Yw8BIuvwoSQ/VsjkCIMoltI/AAAAAAAAC4c/s55PW6xEKn0/s1600-r/nth.png";
var month_format = [, "Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sept", "Oct", "Nov", "Dec"];
var more_text = "View More";
var comments_text = "<span>Post </span>Comment";
var pagenav_prev = "Previous";
var pagenav_next = "Next";
//]]>
</script>
</head>
<body expr:class='data:blog.pageType'>
<!--preloader start-->
<div id='preloader'>
  <div id='loader'>
<span class='loader'><span class='loader-inner'/></span>
</div>
</div>
<!--preloader end-->
&lt;div id=&quot;outer-wrapper&quot; class=&quot;<data:blog.pageType/><b:if cond='data:blog.url == data:blog.homepageUrl'> home</b:if><b:if cond='data:blog.pageType == &quot;static_page&quot;'> item</b:if><b:if cond='data:blog.pageType == &quot;archive&quot;'> index</b:if>&quot;&gt;
<div class='scroll-header' id='head-trigger'>
<div class='scroll-head-wrap row'>
<div class='scrollin-logo'>
  <b:section class='header' id='header' maxwidgets='1' name='Logo &amp; Title' showaddelement='no'>
    <b:widget id='Header1' locked='true' title='vimalprogrammer (Header)' type='Header' version='1'>
      <b:widget-settings>
        <b:widget-setting name='displayUrl'>http://2.bp.blogspot.com/-MzROlqCdQ00/WgF6ynTwnjI/AAAAAAAAEKA/Hf7MDWXOsaY_s0lAivVPeAcob95_jIK9ACK4BGAYYCw/s1600/vcv_blue.png</b:widget-setting>
        <b:widget-setting name='displayHeight'>56</b:widget-setting>
        <b:widget-setting name='sectionWidth'>600</b:widget-setting>
        <b:widget-setting name='useImage'>true</b:widget-setting>
        <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
        <b:widget-setting name='imagePlacement'>REPLACE</b:widget-setting>
        <b:widget-setting name='displayWidth'>317</b:widget-setting>
      </b:widget-settings>
      <b:includable id='main'>
  <b:if cond='data:useImage'>
    <b:if cond='data:imagePlacement == &quot;BEHIND&quot;'>
      <!--
      Show image as background to text. You can't really calculate the width
      reliably in JS because margins are not taken into account by any of
      clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
      width if the user is using shrink to fit.
      This results in a margin-width's worth of pixels being cropped. If the
      user is not using shrink to fit then we expand the header.
      -->
      <b:if cond='data:mobile'>
        <div id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      <b:else/>
        <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                      + &quot;background-position: &quot;                      + data:backgroundPositionStyleStr + &quot;; &quot;                      + data:widthStyleStr                      + &quot;min-height: &quot; + data:height                      + &quot;_height: &quot; + data:height                      + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      </b:if>
    <b:else/>
      <!--Show the image only-->
      <div id='header-inner'>
        <a expr:href='data:blog.homepageUrl' style='display: block'><h1 style='display:none'><data:blog.title/></h1>
          <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' expr:width='data:width' style='display: block'/>
        </a>
        <!--Show the description-->
        <b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
          <b:include name='description'/>
        </b:if>
      </div>
    </b:if>
  <b:else/>
    <!--No header image -->
    <div id='header-inner'>
      <div class='titlewrapper'>
        <h1 class='title'>
          <b:include name='title'/>
        </h1>
      </div>
      <b:include name='description'/>
    </div>
  </b:if>
</b:includable>
      <b:includable id='description'>
  <div class='descriptionwrapper'>
    <p class='description'><span><data:description/></span></p>
  </div>
</b:includable>
      <b:includable id='title'>
  <b:if cond='data:blog.url == data:blog.homepageUrl'>
    <data:title/>
  <b:else/>
    <a expr:href='data:blog.homepageUrl'><data:title/></a>
  </b:if>
</b:includable>
    </b:widget>
  </b:section>
  </div>

<div class='tm-menu'>
<div class='menu-wrap'>
        <b:section class='menu' id='menu' maxwidgets='1' name='Main Menu' showaddelement='yes'>
          <b:widget id='HTML1' locked='false' title='Follow Me' type='HTML'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<br /><div class="separator" style="clear: both; text-align: center;"><div class="separator" style="clear: both; text-align: justify;"><a href="https://1.bp.blogspot.com/-2bveyjNH2S4/XxqzI_wKeKI/AAAAAAAAAAw/X9EfQ6u08NsRf4lpu3MCdTiKBFZ3i2e7QCLcBGAsYHQ/s41/Webp.net-resizeimage.png" style="margin-left: 1em; margin-right: 1em; text-align: center;"><img border="0" data-original-height="41" data-original-width="41" src="https://1.bp.blogspot.com/-2bveyjNH2S4/XxqzI_wKeKI/AAAAAAAAAAw/X9EfQ6u08NsRf4lpu3MCdTiKBFZ3i2e7QCLcBGAsYHQ/s0/Webp.net-resizeimage.png" /></a><a href="https://www.instagram.com/__vimal__official/" style="margin-left: 1em; margin-right: 1em; text-align: center;" target="_blank"><img border="0" data-original-height="39" data-original-width="39" height="38" src="https://1.bp.blogspot.com/-r6GmnRt_uno/Xxq1zxzeFoI/AAAAAAAAABY/AkQOH6a5EYAp_YoknU4UKmPIGFhhEkzVgCLcBGAsYHQ/w38-h38/Webp.net-resizeimage%2B%25284%2529.png" width="38" /></a>;<a href="https://twitter.com/Vimal46701132" target="_blank"><img border="0" data-original-height="41" data-original-width="41" src="https://1.bp.blogspot.com/-QF65MBOSQ-c/Xxq0-BoBoDI/AAAAAAAAABA/cOVXVu-d3A0CH02PQ4-0jOV_9R1OxX6RQCLcBGAsYHQ/s0/Webp.net-resizeimage%2B%25282%2529.png" style="text-align: center;" /></a><a href="https://1.bp.blogspot.com/-1omAjebhmM0/Xxq0xHODXwI/AAAAAAAAAA8/OI8WjoKNFlAN4FFRDuEoxlk3H69nWnNtQCLcBGAsYHQ/s41/Webp.net-resizeimage%2B%25283%2529.png" style="margin-left: 1em; margin-right: 1em;"><img border="0" data-original-height="41" data-original-width="41" src="https://1.bp.blogspot.com/-1omAjebhmM0/Xxq0xHODXwI/AAAAAAAAAA8/OI8WjoKNFlAN4FFRDuEoxlk3H69nWnNtQCLcBGAsYHQ/s0/Webp.net-resizeimage%2B%25283%2529.png" /></a></div><div class="separator" style="clear: both; text-align: left;"><div class="separator" style="clear: both; text-align: center;"><br /></div></div></div>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
  <!-- only display title if it's non-empty -->
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <data:content/>
  </div>

  <b:include name='quickedit'/>
</b:includable>
          </b:widget>
          <b:widget id='LinkList210' locked='true' title='Menu' type='LinkList' version='1'>
            <b:widget-settings>
              <b:widget-setting name='text-9'>Documentation</b:widget-setting>
              <b:widget-setting name='link-9'>https://vimalprogrammer.blogspot.com//2017/11/how-to-setup-sora-cv-blogger-template.html</b:widget-setting>
              <b:widget-setting name='text-8'>Seo Services</b:widget-setting>
              <b:widget-setting name='link-7'>vimal</b:widget-setting>
              <b:widget-setting name='link-8'>http://www.shardawebservices.com</b:widget-setting>
              <b:widget-setting name='text-10'>Download This Template</b:widget-setting>
              <b:widget-setting name='link-5'>http://sora-cv-soratemplate.blogspot.in/p/post-format-and-page-markup.html</b:widget-setting>
              <b:widget-setting name='link-6'>http://www.sorabloggingtips.com/2017/01/how-to-add-sitemap-widget-in-blogspot-blogs.html</b:widget-setting>
              <b:widget-setting name='link-3'>#</b:widget-setting>
              <b:widget-setting name='link-4'>#</b:widget-setting>
              <b:widget-setting name='text-1'>_Multi DropDown</b:widget-setting>
              <b:widget-setting name='text-0'>Features</b:widget-setting>
              <b:widget-setting name='text-3'>__DropDown 2</b:widget-setting>
              <b:widget-setting name='text-2'>__DropDown 1</b:widget-setting>
              <b:widget-setting name='text-5'>_ShortCodes</b:widget-setting>
              <b:widget-setting name='text-4'>__DropDown 3</b:widget-setting>
              <b:widget-setting name='text-7'>_Error Page</b:widget-setting>
              <b:widget-setting name='text-6'>_Sitemap</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='link-1'>#</b:widget-setting>
              <b:widget-setting name='link-2'>#</b:widget-setting>
              <b:widget-setting name='link-0'>#</b:widget-setting>
              <b:widget-setting name='link-10'>http://www.soratemplates.com/2017/11/sora-cv-blogger-templates.html</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
            <div class='widget-content'>
              <ul itemscope='' itemtype='http://schema.org/SiteNavigationElement'> 
                <li><a expr:href='data:blog.homepageUrl'>Home</a></li>
                <b:loop values='data:links' var='link'>
                  <li itemprop='name'><a expr:href='data:link.target' itemprop='url'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:includable>
          </b:widget>
        </b:section>
	<div class='menu-mobile'/>
	
  </div>
      </div>
  
</div></div>
  <div style='clear: both;'/>
<b:if cond='data:blog.pageType != &quot;static_page&quot;'>
<b:if cond='data:blog.pageType!= &quot;item&quot;'>
<b:if cond='data:blog.pageType != &quot;error_page&quot;'>
<div id='header-wrapper'>
<div class='background-container' id='#background-container'>
 


</div>

<div class='fenix-head'>
<div class='fenix-sub-head wow fadeInUp hero-row' style='visibility: visible;animation-delay: 1.2s;'>
<div class='sora-author-box'>

<div class='sora-author-box-image'><img alt='Author Image' class='avatar avatar-60 photo' src='https://1.bp.blogspot.com/-xDkUGm3z4Yk/XxqqdDr9cEI/AAAAAAAAAAk/PGErp1EGXscKINZ9qIEX4f2b9sYeLBZxACLcBGAsYHQ/s320/Vimal.jpg'/></div>  
<div class='sora-author-box-text'>
<div class='sora-author-box-text-head'>
<span class='hello-txt'>Hello</span>
<h2 class='profile-title'><span>I&#39;m</span> Vimal M</h2>
<h3 class='profile-position'>Software developer and Programmer</h3>
  </div>
<div class='sora-author-box-text-details'>
<ul class='profile-list'>
    <li class='clearfix'>
        <strong class='list-title'>Age</strong>
        <span class='cont'>19</span>
    </li>
    <li class='clearfix'>
        <strong class='list-title'>Address</strong>
        <span class='cont'>130/1, Melavayalur street, Kuhoor post, Lalgudi, TRICHY</span>
    </li>
    <li class='clearfix'>
        <strong class='list-title'>E-mail</strong>
        <span class='cont'><a href='mailto:vimaldeveloper19@gmail.com'>vimaldeveloper19@gmail.com</a></span>
    </li>
    <li class='clearfix'>
        <strong class='list-title'>Phone</strong>
        <span class='cont'><a href='tel:+91 7092145356'>+91 7092145356</a></span>
    </li>
    <li class='clearfix'>
        <strong class='list-title'>Qualification</strong>
        <span class='cont'>Currently proceeding Bachelor of Engineering in the stream of Computer Science at K.Ramakrishnan College Of Technology.</span>
    </li>

</ul>
  </div>
<div style='clear: both;'/>
</div></div>
<div style='clear: both;'/>
<div class='social-head'>
<b:section class='top-bar-social blue' id='header social widget' maxwidgets='1' name='Top Social Widget' showaddelement='no'>
  <b:widget id='LinkList230' locked='true' title='Social Media Icons' type='LinkList' version='1'>
    <b:widget-settings>
      <b:widget-setting name='link-5'>#</b:widget-setting>
      <b:widget-setting name='link-3'>#</b:widget-setting>
      <b:widget-setting name='link-4'>#</b:widget-setting>
      <b:widget-setting name='text-1'>twitter</b:widget-setting>
      <b:widget-setting name='text-0'>facebook</b:widget-setting>
      <b:widget-setting name='text-3'>instagram</b:widget-setting>
      <b:widget-setting name='text-2'>gplus</b:widget-setting>
      <b:widget-setting name='text-5'>linkedin</b:widget-setting>
      <b:widget-setting name='text-4'>pinterest</b:widget-setting>
      <b:widget-setting name='sorting'>NONE</b:widget-setting>
      <b:widget-setting name='link-1'>#</b:widget-setting>
      <b:widget-setting name='link-2'>#</b:widget-setting>
      <b:widget-setting name='link-0'>#</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
            <div class='widget-content'>
              <ul id='social'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:class='data:link.name' expr:href='data:link.target' expr:title='data:link.name'/></li>
                </b:loop>
              </ul>
            </div>

          </b:includable>
  </b:widget>
</b:section>
  </div>
  </div>
  </div>
</div>
<div style='clear: both;'/>
  </b:if>
  </b:if>
  </b:if>
<b:if cond='data:blog.pageType != &quot;static_page&quot;'>
<b:if cond='data:blog.pageType!= &quot;item&quot;'>
<b:if cond='data:blog.pageType != &quot;error_page&quot;'>
<div class='sora-cv-author-details wow slideInUp row' style='visibility: visible;animation-delay: 1.5s;'>
<div class='card-content'>
    <!-- ABOUT PARAGRAPH -->
    <p>
        Hello! I&#8217;m Vimal M. Junior Software Developer. Certified with many Programming Languages.Having an in-depth knowledge including advanced HTML5, CSS, Java, JavaScript, Python, C and C++.
    </p>
</div>


                    </div>

<div style='clear: both;'/>

<div class='sora-special-box wow slideInUp' id='section-2'>
<div class='special-wrap row'>
<div class='special-title wow fadeInUp animated' style='visibility: visible;'>
  <h4><i class='lnr lnr-chart-bars'/>Professional Skills</h4>
  </div>
<div style='clear: both;'/>
<div class='special-wrap-inner'>
<div class='skills'>
   <!-- skill -->
  <dl>
    <dt>HTML</dt>
    <dd class='skill-percent html' data-percent='90'/>
    <dt>CSS</dt>
    <dd class='skill-percent css' data-percent='85'/>
    <dt>Python</dt>
    <dd class='skill-percent jquery' data-percent='80'/>
    <dt>Javascript</dt>
    <dd class='skill-percent javascript' data-percent='50'/>
  </dl>
   <!-- #skill -->
</div>
<div class='skill-details'>
<div class='skill-wrapper'>
    <div class='skill-progress'>
        <div class='circle'>
            <div class='mask'/>
            <div class='mask'/>
        </div>
        <div class='inset'>
            <div class='numbers'/>
        </div>
    </div>


    <div class='skill-progress'>
        <div class='circle'>
            <div class='mask'/>
            <div class='mask'/>
        </div>
        <div class='inset'>
            <div class='numbers'/>
        </div>
    </div>


    <div class='skill-progress'>
        <div class='circle'>
            <div class='mask'/>
            <div class='mask'/>
        </div>
        <div class='inset'>
            <div class='numbers'/>
        </div>
    </div>

</div>
<div style='clear: both;'/>
  </div>
  </div>
  </div></div>

  <div style='clear:both;'/>
<div class='sora-cv-hobby-details wow zoomIn row' style='visibility: visible;'>
<div class='hobby-title'>
<h4><i class='lnr lnr-heart'/>My Interest</h4>
</div>
 <div style='clear:both;'/>
<div class='sora-cv-hobby-details-inner'>
<div class='card-content'>
<!-- Hobby PARAGRAPH -->
<p>
      First of all I love music, country music is my favorite. Love watching football, cricket, movies and playing games with my buddies. I spend quite a lot of time in traveling and playing cricket, these keeps me fresh for working environment.
    </p>
</div>

  


<div style='clear: both;'/>
<div class='map-me-full wow bounceInUp' style='visibility: visible;'>
 <div id='map'/>
    <script>
      function initMap() {
        var uluru = {lat: 51.5074, lng: 0.1278};
        var map = new google.maps.Map(document.getElementById(&#39;map&#39;), {
          zoom: 4,
          center: uluru
        });
        var marker = new google.maps.Marker({
          position: uluru,
          map: map
        });
      }
    </script>
<script src='https://maps.googleapis.com/maps/api/js?key=AIzaSyBtM96UHgaqhuIOQ0CyINA6rGpYqwonosI&amp;callback=initMap'>
    </script>
  </div>
<div style='clear: both;'/>
<div class='insta-wrap' id='section-1'>
<div class='contact-title'>
<h4><i class='lnr lnr-phone'/> Get in Touch</h4>
</div>
  <div style='clear:both'/>
<div class='contact_list_wrapper'>
		</div>
 <div style='clear:both'/>
<div class='row' id='sora_blogger_cntct_form'>
<div class='wrap-me wow fadeInLeft' data-wow-delay='0.2s' style='visibility: visible;'>
<b:section class='sora-contact-widget' id='Contact Widget' maxwidgets='1' name='Contact Form Widget' showaddelement='no'>
  <b:widget id='ContactForm1' locked='false' title='Contact form' type='ContactForm' version='1'>
    <b:includable id='main'>
  <div class='contact-form-widget'>
    <div class='form'>
      <form name='contact-form'>
        <p/>
        <span class='name-bg'>Name*</span>
        <br/>
        <input class='contact-form-name' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' name='name' size='30' type='text' value=''/>
        <p/>
        <span class='email-bg'>Email*</span>
        <br/>
        <input class='contact-form-email' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' name='email' size='30' type='text' value=''/>
        <p/>
        <span class='message-bg'>Message*</span>
        <br/>
        <textarea class='contact-form-email-message' cols='25' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' name='email-message' rows='5'/>
        <p/>
<span class='send-bg'>
        <input class='contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/></span>
<span class='clear-bg'><input class='contact-form-button contact-form-button-submit clear-button' type='reset' value='Clear'/></span>
        <p/>
    <div style='max-width: 100%; text-align: center; width: 100%;'>
<div class='contact-form-error-message' id='ContactForm1_contact-form-error-message'>
</div>
<div class='contact-form-success-message' id='ContactForm1_contact-form-success-message'>
</div>
</div>
      </form>
    </div>
  </div>
  <b:include name='quickedit'/>
</b:includable>
  </b:widget>
</b:section>
<br/>
<h1 class='con-title'><u>Reach me on</u></h1>
<br/><div class='separator' style='clear: both; text-align: center;'><div class='separator' style='clear: both; text-align: justify;'><a href='https://www.facebook.com/vimal.programmer' style='margin-left: 1em; margin-right: 1em; text-align: center;' target='_blank'><img border='0' data-original-height='41' data-original-width='41' src='https://1.bp.blogspot.com/-2bveyjNH2S4/XxqzI_wKeKI/AAAAAAAAAAw/X9EfQ6u08NsRf4lpu3MCdTiKBFZ3i2e7QCLcBGAsYHQ/s0/Webp.net-resizeimage.png'/></a><a href='https://www.instagram.com/__vimal__official/' style='margin-left: 1em; margin-right: 1em; text-align: center;' target='_blank'><img border='0' data-original-height='39' data-original-width='39' height='38' src='https://1.bp.blogspot.com/-r6GmnRt_uno/Xxq1zxzeFoI/AAAAAAAAABY/AkQOH6a5EYAp_YoknU4UKmPIGFhhEkzVgCLcBGAsYHQ/w38-h38/Webp.net-resizeimage%2B%25284%2529.png' width='38'/></a><a href='https://twitter.com/Vimal46701132' target='_blank'><img border='0' data-original-height='41' data-original-width='41' src='https://1.bp.blogspot.com/-QF65MBOSQ-c/Xxq0-BoBoDI/AAAAAAAAABA/cOVXVu-d3A0CH02PQ4-0jOV_9R1OxX6RQCLcBGAsYHQ/s0/Webp.net-resizeimage%2B%25282%2529.png' style='text-align: center;'/></a><a href='mailto:vimaldeveloper19@gmail.com' style='margin-left: 1em; margin-right: 1em;' target='_blank'><img border='0' data-original-height='41' data-original-width='41' src='https://1.bp.blogspot.com/-1omAjebhmM0/Xxq0xHODXwI/AAAAAAAAAA8/OI8WjoKNFlAN4FFRDuEoxlk3H69nWnNtQCLcBGAsYHQ/s0/Webp.net-resizeimage%2B%25283%2529.png'/></a></div><div class='separator' style='clear: both; text-align: left;'><div class='separator' style='clear: both; text-align: center;'><br/></div></div></div>
</div><div class='map-me wow fadeInRight' data-wow-delay='0s' style='visibility: visible;'>
 <div class='contact-other'>
<h2 class='con-title'><u>Feel Free To Contact</u></h2>

<ul class='con-list'>
<li><i class='lnr lnr-map'/>130/1,Kuhoor,Lalgudi,Trichy.</li>
<li><i class='lnr lnr-phone'/>+91 7092145356, +91 9095472117</li>
<li><i class='lnr lnr-envelope'/>vimalprogrammer@gmail.com</li>
<li><i class='lnr lnr-earth'/>vimalmprogrammer.blogspot.com</li>
</ul>  
</div>
  </div>
</div>
</div>
  </div>
  </div>
  </b:if></b:if></b:if>
<div style='clear: both;'/>
<div class='bot-bar-menu'>


<div class='bot-menu-wrap row'>
 

 <div class='jugas_footer_copyright'>
                      Created By <a id='mycontent' rel='dofollow' title='Free Blogger Templates'>Vimal </a> | Distributed By <b><a rel='dofollow' style='color:#f76e0a;' target='_blank'>Blogger Templates</a></b>
                    </div>

 <b:section class='bottom-bar-social blue' id='Footer social widget' maxwidgets='1' name='Footer Social Widget' showaddelement='no'>
   <b:widget id='LinkList236' locked='true' title='Social Media Icons' type='LinkList' version='1'>
     <b:widget-settings>
       <b:widget-setting name='link-3'>#</b:widget-setting>
       <b:widget-setting name='sorting'>NONE</b:widget-setting>
       <b:widget-setting name='link-4'>#</b:widget-setting>
       <b:widget-setting name='text-1'>twitter</b:widget-setting>
       <b:widget-setting name='link-1'>#</b:widget-setting>
       <b:widget-setting name='text-0'>facebook</b:widget-setting>
       <b:widget-setting name='link-2'>#</b:widget-setting>
       <b:widget-setting name='text-3'>bloglovin</b:widget-setting>
       <b:widget-setting name='link-0'>#</b:widget-setting>
       <b:widget-setting name='text-2'>gplus</b:widget-setting>
       <b:widget-setting name='text-4'>instagram</b:widget-setting>
     </b:widget-settings>
     <b:includable id='main'>
            <div class='widget-content'>
              <ul id='social'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:class='data:link.name' expr:href='data:link.target' expr:title='data:link.name'/></li>
                </b:loop>
              </ul>
            </div>
          </b:includable>
   </b:widget>
 </b:section>
</div>
  </div>
                   
               
              
                    
       
&lt;/div&gt;
<script>
/*<![CDATA[*/
/*! WOW wow.js - v1.3.0 - 2016-10-04
* https://wowjs.uk
* Copyright (c) 2016 Thomas Grainger; Licensed MIT */!function(a,b){if("function"==typeof define&&define.amd)define(["module","exports"],b);else if("undefined"!=typeof exports)b(module,exports);else{var c={exports:{}};b(c,c.exports),a.WOW=c.exports}}(this,function(a,b){"use strict";function c(a,b){if(!(a instanceof b))throw new TypeError("Cannot call a class as a function")}function d(a,b){return b.indexOf(a)>=0}function e(a,b){for(var c in b)if(null==a[c]){var d=b[c];a[c]=d}return a}function f(a){return/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(a)}function g(a){var b=arguments.length<=1||void 0===arguments[1]?!1:arguments[1],c=arguments.length<=2||void 0===arguments[2]?!1:arguments[2],d=arguments.length<=3||void 0===arguments[3]?null:arguments[3],e=void 0;return null!=document.createEvent?(e=document.createEvent("CustomEvent"),e.initCustomEvent(a,b,c,d)):null!=document.createEventObject?(e=document.createEventObject(),e.eventType=a):e.eventName=a,e}function h(a,b){null!=a.dispatchEvent?a.dispatchEvent(b):b in(null!=a)?a[b]():"on"+b in(null!=a)&&a["on"+b]()}function i(a,b,c){null!=a.addEventListener?a.addEventListener(b,c,!1):null!=a.attachEvent?a.attachEvent("on"+b,c):a[b]=c}function j(a,b,c){null!=a.removeEventListener?a.removeEventListener(b,c,!1):null!=a.detachEvent?a.detachEvent("on"+b,c):delete a[b]}function k(){return"innerHeight"in window?window.innerHeight:document.documentElement.clientHeight}Object.defineProperty(b,"__esModule",{value:!0});var l,m,n=function(){function a(a,b){for(var c=0;c<b.length;c++){var d=b[c];d.enumerable=d.enumerable||!1,d.configurable=!0,"value"in d&&(d.writable=!0),Object.defineProperty(a,d.key,d)}}return function(b,c,d){return c&&a(b.prototype,c),d&&a(b,d),b}}(),o=window.WeakMap||window.MozWeakMap||function(){function a(){c(this,a),this.keys=[],this.values=[]}return n(a,[{key:"get",value:function(a){for(var b=0;b<this.keys.length;b++){var c=this.keys[b];if(c===a)return this.values[b]}}},{key:"set",value:function(a,b){for(var c=0;c<this.keys.length;c++){var d=this.keys[c];if(d===a)return this.values[c]=b,this}return this.keys.push(a),this.values.push(b),this}}]),a}(),p=window.MutationObserver||window.WebkitMutationObserver||window.MozMutationObserver||(m=l=function(){function a(){c(this,a),"undefined"!=typeof console&&null!==console&&(console.warn("MutationObserver is not supported by your browser."),console.warn("WOW.js cannot detect dom mutations, please call .sync() after loading new content."))}return n(a,[{key:"observe",value:function(){}}]),a}(),l.notSupported=!0,m),q=window.getComputedStyle||function(a){var b=/(\-([a-z]){1})/g;return{getPropertyValue:function(c){"float"===c&&(c="styleFloat"),b.test(c)&&c.replace(b,function(a,b){return b.toUpperCase()});var d=a.currentStyle;return(null!=d?d[c]:void 0)||null}}},r=function(){function a(){var b=arguments.length<=0||void 0===arguments[0]?{}:arguments[0];c(this,a),this.defaults={boxClass:"wow",animateClass:"animated",offset:0,mobile:!0,live:!0,callback:null,scrollContainer:null,resetAnimation:!0},this.animate=function(){return"requestAnimationFrame"in window?function(a){return window.requestAnimationFrame(a)}:function(a){return a()}}(),this.vendors=["moz","webkit"],this.start=this.start.bind(this),this.resetAnimation=this.resetAnimation.bind(this),this.scrollHandler=this.scrollHandler.bind(this),this.scrollCallback=this.scrollCallback.bind(this),this.scrolled=!0,this.config=e(b,this.defaults),null!=b.scrollContainer&&(this.config.scrollContainer=document.querySelector(b.scrollContainer)),this.animationNameCache=new o,this.wowEvent=g(this.config.boxClass)}return n(a,[{key:"init",value:function(){this.element=window.document.documentElement,d(document.readyState,["interactive","complete"])?this.start():i(document,"DOMContentLoaded",this.start),this.finished=[]}},{key:"start",value:function(){var a=this;if(this.stopped=!1,this.boxes=[].slice.call(this.element.querySelectorAll("."+this.config.boxClass)),this.all=this.boxes.slice(0),this.boxes.length)if(this.disabled())this.resetStyle();else for(var b=0;b<this.boxes.length;b++){var c=this.boxes[b];this.applyStyle(c,!0)}if(this.disabled()||(i(this.config.scrollContainer||window,"scroll",this.scrollHandler),i(window,"resize",this.scrollHandler),this.interval=setInterval(this.scrollCallback,50)),this.config.live){var d=new p(function(b){for(var c=0;c<b.length;c++)for(var d=b[c],e=0;e<d.addedNodes.length;e++){var f=d.addedNodes[e];a.doSync(f)}});d.observe(document.body,{childList:!0,subtree:!0})}}},{key:"stop",value:function(){this.stopped=!0,j(this.config.scrollContainer||window,"scroll",this.scrollHandler),j(window,"resize",this.scrollHandler),null!=this.interval&&clearInterval(this.interval)}},{key:"sync",value:function(){p.notSupported&&this.doSync(this.element)}},{key:"doSync",value:function(a){if("undefined"!=typeof a&&null!==a||(a=this.element),1===a.nodeType){a=a.parentNode||a;for(var b=a.querySelectorAll("."+this.config.boxClass),c=0;c<b.length;c++){var e=b[c];d(e,this.all)||(this.boxes.push(e),this.all.push(e),this.stopped||this.disabled()?this.resetStyle():this.applyStyle(e,!0),this.scrolled=!0)}}}},{key:"show",value:function(a){return this.applyStyle(a),a.className=a.className+" "+this.config.animateClass,null!=this.config.callback&&this.config.callback(a),h(a,this.wowEvent),this.config.resetAnimation&&(i(a,"animationend",this.resetAnimation),i(a,"oanimationend",this.resetAnimation),i(a,"webkitAnimationEnd",this.resetAnimation),i(a,"MSAnimationEnd",this.resetAnimation)),a}},{key:"applyStyle",value:function(a,b){var c=this,d=a.getAttribute("data-wow-duration"),e=a.getAttribute("data-wow-delay"),f=a.getAttribute("data-wow-iteration");return this.animate(function(){return c.customStyle(a,b,d,e,f)})}},{key:"resetStyle",value:function(){for(var a=0;a<this.boxes.length;a++){var b=this.boxes[a];b.style.visibility="visible"}}},{key:"resetAnimation",value:function(a){if(a.type.toLowerCase().indexOf("animationend")>=0){var b=a.target||a.srcElement;b.className=b.className.replace(this.config.animateClass,"").trim()}}},{key:"customStyle",value:function(a,b,c,d,e){return b&&this.cacheAnimationName(a),a.style.visibility=b?"hidden":"visible",c&&this.vendorSet(a.style,{animationDuration:c}),d&&this.vendorSet(a.style,{animationDelay:d}),e&&this.vendorSet(a.style,{animationIterationCount:e}),this.vendorSet(a.style,{animationName:b?"none":this.cachedAnimationName(a)}),a}},{key:"vendorSet",value:function(a,b){for(var c in b)if(b.hasOwnProperty(c)){var d=b[c];a[""+c]=d;for(var e=0;e<this.vendors.length;e++){var f=this.vendors[e];a[""+f+c.charAt(0).toUpperCase()+c.substr(1)]=d}}}},{key:"vendorCSS",value:function(a,b){for(var c=q(a),d=c.getPropertyCSSValue(b),e=0;e<this.vendors.length;e++){var f=this.vendors[e];d=d||c.getPropertyCSSValue("-"+f+"-"+b)}return d}},{key:"animationName",value:function(a){var b=void 0;try{b=this.vendorCSS(a,"animation-name").cssText}catch(c){b=q(a).getPropertyValue("animation-name")}return"none"===b?"":b}},{key:"cacheAnimationName",value:function(a){return this.animationNameCache.set(a,this.animationName(a))}},{key:"cachedAnimationName",value:function(a){return this.animationNameCache.get(a)}},{key:"scrollHandler",value:function(){this.scrolled=!0}},{key:"scrollCallback",value:function(){if(this.scrolled){this.scrolled=!1;for(var a=[],b=0;b<this.boxes.length;b++){var c=this.boxes[b];if(c){if(this.isVisible(c)){this.show(c);continue}a.push(c)}}this.boxes=a,this.boxes.length||this.config.live||this.stop()}}},{key:"offsetTop",value:function(a){for(;void 0===a.offsetTop;)a=a.parentNode;for(var b=a.offsetTop;a.offsetParent;)a=a.offsetParent,b+=a.offsetTop;return b}},{key:"isVisible",value:function(a){var b=a.getAttribute("data-wow-offset")||this.config.offset,c=this.config.scrollContainer&&this.config.scrollContainer.scrollTop||window.pageYOffset,d=c+Math.min(this.element.clientHeight,k())-b,e=this.offsetTop(a),f=e+a.clientHeight;return d>=e&&f>=c}},{key:"disabled",value:function(){return!this.config.mobile&&f(navigator.userAgent)}}]),a}();b["default"]=r,a.exports=b["default"]});

  new WOW().init();


// this has nothing to do with the animation, just forces the window to be a size that allows a scroll
var containerHeight = $(window).height() / 2;

$('.spacer').css("height", containerHeight);

// Find the height of the previous section, half it so when you have scrolled more than half past the section, it triggers the animation
var x = $('.skills').prev().height() / 4;

$(window).scroll(function() {
  // checks to see if you have scrolled far enough down to activate the animation
  if ($(window).scrollTop() >= x) {
    //find each element with the class .skill-percent
    $('.skill-percent').each(function() {
      // animate
      $(this).animate({
        //finds the width from the data-percent attribute
        width: $(this).data('percent') + '%'
      }, 1000);
    });
  }
});

/*]]>*/
</script>

<script type='text/javascript'>
//<![CDATA[

/*!
    SlickNav Responsive Mobile Menu
    (c) 2014 Josh Cope
    licensed under MIT
*/
;(function(e,t,n){function o(t,n){this.element=t;this.settings=e.extend({},r,n);this._defaults=r;this._name=i;this.init()}var r={label:"MENU",duplicate:true,duration:200,easingOpen:"swing",easingClose:"swing",closedSymbol:"&#9658;",openedSymbol:"&#9660;",prependTo:"body",parentTag:"a",closeOnClick:false,allowParentLinks:false,nestedParentLinks:true,showChildren:false,init:function(){},open:function(){},close:function(){}},i="slicknav",s="slicknav";o.prototype.init=function(){var n=this;var r=e(this.element);var i=this.settings;if(i.duplicate){n.mobileNav=r.clone();n.mobileNav.removeAttr("id");n.mobileNav.find("*").each(function(t,n){e(n).removeAttr("id")})}else n.mobileNav=r;var o=s+"_icon";if(i.label===""){o+=" "+s+"_no-text"}if(i.parentTag=="a"){i.parentTag='a href="#"'}n.mobileNav.attr("class",s+"_nav");var u=e('<div class="'+s+'_menu"></div>');n.btn=e("<"+i.parentTag+' aria-haspopup="true" tabindex="0" class="'+s+"_btn "+s+'_collapsed"><span class="'+s+'_menutxt">'+i.label+'</span><span class="'+o+'"><span class="'+s+'_icon-bar"></span><span class="'+s+'_icon-bar"></span><span class="'+s+'_icon-bar"></span></span></a>');e(u).append(n.btn);e(i.prependTo).prepend(u);u.append(n.mobileNav);var a=n.mobileNav.find("li");e(a).each(function(){var t=e(this);var r={};r.children=t.children("ul").attr("role","menu");t.data("menu",r);if(r.children.length>0){var o=t.contents();var u=false;var a=[];e(o).each(function(){if(!e(this).is("ul")){a.push(this)}else{return false}if(e(this).is("a")){u=true}});var f=e("<"+i.parentTag+' role="menuitem" aria-haspopup="true" tabindex="-1" class="'+s+'_item"/>');if(!i.allowParentLinks||i.nestedParentLinks||!u){var l=e(a).wrapAll(f).parent();l.addClass(s+"_row")}else e(a).wrapAll('<span class="'+s+"_parent-link "+s+'_row"/>').parent();t.addClass(s+"_collapsed");t.addClass(s+"_parent");var c=e('<span class="'+s+'_arrow">'+i.closedSymbol+"</span>");if(i.allowParentLinks&&!i.nestedParentLinks&&u)c=c.wrap(f).parent();e(a).last().after(c)}else if(t.children().length===0){t.addClass(s+"_txtnode")}t.children("a").attr("role","menuitem").click(function(t){if(i.closeOnClick&&!e(t.target).parent().closest("li").hasClass(s+"_parent"))e(n.btn).click()});if(i.closeOnClick&&i.allowParentLinks){t.children("a").children("a").click(function(t){e(n.btn).click()});t.find("."+s+"_parent-link a:not(."+s+"_item)").click(function(t){e(n.btn).click()})}});e(a).each(function(){var t=e(this).data("menu");if(!i.showChildren){n._visibilityToggle(t.children,null,false,null,true)}});n._visibilityToggle(n.mobileNav,null,false,"init",true);n.mobileNav.attr("role","menu");e(t).mousedown(function(){n._outlines(false)});e(t).keyup(function(){n._outlines(true)});e(n.btn).click(function(e){e.preventDefault();n._menuToggle()});n.mobileNav.on("click","."+s+"_item",function(t){t.preventDefault();n._itemClick(e(this))});e(n.btn).keydown(function(e){var t=e||event;if(t.keyCode==13){e.preventDefault();n._menuToggle()}});n.mobileNav.on("keydown","."+s+"_item",function(t){var r=t||event;if(r.keyCode==13){t.preventDefault();n._itemClick(e(t.target))}});if(i.allowParentLinks&&i.nestedParentLinks){e("."+s+"_item a").click(function(e){e.stopImmediatePropagation()})}};o.prototype._menuToggle=function(e){var t=this;var n=t.btn;var r=t.mobileNav;if(n.hasClass(s+"_collapsed")){n.removeClass(s+"_collapsed");n.addClass(s+"_open")}else{n.removeClass(s+"_open");n.addClass(s+"_collapsed")}n.addClass(s+"_animating");t._visibilityToggle(r,n.parent(),true,n)};o.prototype._itemClick=function(e){var t=this;var n=t.settings;var r=e.data("menu");if(!r){r={};r.arrow=e.children("."+s+"_arrow");r.ul=e.next("ul");r.parent=e.parent();if(r.parent.hasClass(s+"_parent-link")){r.parent=e.parent().parent();r.ul=e.parent().next("ul")}e.data("menu",r)}if(r.parent.hasClass(s+"_collapsed")){r.arrow.html(n.openedSymbol);r.parent.removeClass(s+"_collapsed");r.parent.addClass(s+"_open");r.parent.addClass(s+"_animating");t._visibilityToggle(r.ul,r.parent,true,e)}else{r.arrow.html(n.closedSymbol);r.parent.addClass(s+"_collapsed");r.parent.removeClass(s+"_open");r.parent.addClass(s+"_animating");t._visibilityToggle(r.ul,r.parent,true,e)}};o.prototype._visibilityToggle=function(t,n,r,i,o){var u=this;var a=u.settings;var f=u._getActionItems(t);var l=0;if(r)l=a.duration;if(t.hasClass(s+"_hidden")){t.removeClass(s+"_hidden");t.slideDown(l,a.easingOpen,function(){e(i).removeClass(s+"_animating");e(n).removeClass(s+"_animating");if(!o){a.open(i)}});t.attr("aria-hidden","false");f.attr("tabindex","0");u._setVisAttr(t,false)}else{t.addClass(s+"_hidden");t.slideUp(l,this.settings.easingClose,function(){t.attr("aria-hidden","true");f.attr("tabindex","-1");u._setVisAttr(t,true);t.hide();e(i).removeClass(s+"_animating");e(n).removeClass(s+"_animating");if(!o)a.close(i);else if(i=="init")a.init()})}};o.prototype._setVisAttr=function(t,n){var r=this;var i=t.children("li").children("ul").not("."+s+"_hidden");if(!n){i.each(function(){var t=e(this);t.attr("aria-hidden","false");var i=r._getActionItems(t);i.attr("tabindex","0");r._setVisAttr(t,n)})}else{i.each(function(){var t=e(this);t.attr("aria-hidden","true");var i=r._getActionItems(t);i.attr("tabindex","-1");r._setVisAttr(t,n)})}};o.prototype._getActionItems=function(e){var t=e.data("menu");if(!t){t={};var n=e.children("li");var r=n.find("a");t.links=r.add(n.find("."+s+"_item"));e.data("menu",t)}return t.links};o.prototype._outlines=function(t){if(!t){e("."+s+"_item, ."+s+"_btn").css("outline","none")}else{e("."+s+"_item, ."+s+"_btn").css("outline","")}};o.prototype.toggle=function(){var e=this;e._menuToggle()};o.prototype.open=function(){var e=this;if(e.btn.hasClass(s+"_collapsed")){e._menuToggle()}};o.prototype.close=function(){var e=this;if(e.btn.hasClass(s+"_open")){e._menuToggle()}};e.fn[i]=function(t){var n=arguments;if(t===undefined||typeof t==="object"){return this.each(function(){if(!e.data(this,"plugin_"+i)){e.data(this,"plugin_"+i,new o(this,t))}})}else if(typeof t==="string"&&t[0]!=="_"&&t!=="init"){var r;this.each(function(){var s=e.data(this,"plugin_"+i);if(s instanceof o&&typeof s[t]==="function"){r=s[t].apply(s,Array.prototype.slice.call(n,1))}});return r!==undefined?r:this}}})(jQuery,document,window)

!function($){"use strict";var Typed=function(el,options){this.el=$(el);this.options=$.extend({},$.fn.typed.defaults,options);this.isInput=this.el.is("input");this.attr=this.options.attr;this.showCursor=this.isInput?false:this.options.showCursor;this.elContent=this.attr?this.el.attr(this.attr):this.el.text();this.contentType=this.options.contentType;this.typeSpeed=this.options.typeSpeed;this.startDelay=this.options.startDelay;this.backSpeed=this.options.backSpeed;this.backDelay=this.options.backDelay;this.stringsElement=this.options.stringsElement;this.strings=this.options.strings;this.strPos=0;this.arrayPos=0;this.stopNum=0;this.loop=this.options.loop;this.loopCount=this.options.loopCount;this.curLoop=0;this.stop=false;this.cursorChar=this.options.cursorChar;this.shuffle=this.options.shuffle;this.sequence=[];this.build()};Typed.prototype={constructor:Typed,init:function(){var self=this;self.timeout=setTimeout(function(){for(var i=0;i<self.strings.length;++i)self.sequence[i]=i;if(self.shuffle)self.sequence=self.shuffleArray(self.sequence);self.typewrite(self.strings[self.sequence[self.arrayPos]],self.strPos)},self.startDelay)},build:function(){var self=this;if(this.showCursor===true){this.cursor=$('<span class="typed-cursor">'+this.cursorChar+"</span>");this.el.after(this.cursor)}if(this.stringsElement){this.strings=[];this.stringsElement.hide();console.log(this.stringsElement.children());var strings=this.stringsElement.children();$.each(strings,function(key,value){self.strings.push($(value).html())})}this.init()},typewrite:function(curString,curStrPos){if(this.stop===true){return}var humanize=Math.round(Math.random()*(100-30))+this.typeSpeed;var self=this;self.timeout=setTimeout(function(){var charPause=0;var substr=curString.substr(curStrPos);if(substr.charAt(0)==="^"){var skip=1;if(/^\^\d+/.test(substr)){substr=/\d+/.exec(substr)[0];skip+=substr.length;charPause=parseInt(substr)}curString=curString.substring(0,curStrPos)+curString.substring(curStrPos+skip)}if(self.contentType==="html"){var curChar=curString.substr(curStrPos).charAt(0);if(curChar==="<"||curChar==="&"){var tag="";var endTag="";if(curChar==="<"){endTag=">"}else{endTag=";"}while(curString.substr(curStrPos+1).charAt(0)!==endTag){tag+=curString.substr(curStrPos).charAt(0);curStrPos++;if(curStrPos+1>curString.length){break}}curStrPos++;tag+=endTag}}self.timeout=setTimeout(function(){if(curStrPos===curString.length){self.options.onStringTyped(self.arrayPos);if(self.arrayPos===self.strings.length-1){self.options.callback();self.curLoop++;if(self.loop===false||self.curLoop===self.loopCount)return}self.timeout=setTimeout(function(){self.backspace(curString,curStrPos)},self.backDelay)}else{if(curStrPos===0){self.options.preStringTyped(self.arrayPos)}var nextString=curString.substr(0,curStrPos+1);if(self.attr){self.el.attr(self.attr,nextString)}else{if(self.isInput){self.el.val(nextString)}else if(self.contentType==="html"){self.el.html(nextString)}else{self.el.text(nextString)}}curStrPos++;self.typewrite(curString,curStrPos)}},charPause)},humanize)},backspace:function(curString,curStrPos){if(this.stop===true){return}var humanize=Math.round(Math.random()*(100-30))+this.backSpeed;var self=this;self.timeout=setTimeout(function(){if(self.contentType==="html"){if(curString.substr(curStrPos).charAt(0)===">"){var tag="";while(curString.substr(curStrPos-1).charAt(0)!=="<"){tag-=curString.substr(curStrPos).charAt(0);curStrPos--;if(curStrPos<0){break}}curStrPos--;tag+="<"}}var nextString=curString.substr(0,curStrPos);if(self.attr){self.el.attr(self.attr,nextString)}else{if(self.isInput){self.el.val(nextString)}else if(self.contentType==="html"){self.el.html(nextString)}else{self.el.text(nextString)}}if(curStrPos>self.stopNum){curStrPos--;self.backspace(curString,curStrPos)}else if(curStrPos<=self.stopNum){self.arrayPos++;if(self.arrayPos===self.strings.length){self.arrayPos=0;if(self.shuffle)self.sequence=self.shuffleArray(self.sequence);self.init()}else self.typewrite(self.strings[self.sequence[self.arrayPos]],curStrPos)}},humanize)},shuffleArray:function(array){var tmp,current,top=array.length;if(top)while(--top){current=Math.floor(Math.random()*(top+1));tmp=array[current];array[current]=array[top];array[top]=tmp}return array},reset:function(){var self=this;clearInterval(self.timeout);var id=this.el.attr("id");this.el.empty();if(typeof this.cursor!=="undefined"){this.cursor.remove()}this.strPos=0;this.arrayPos=0;this.curLoop=0;this.options.resetCallback()}};$.fn.typed=function(option){return this.each(function(){var $this=$(this),data=$this.data("typed"),options=typeof option=="object"&&option;if(data){data.reset()}$this.data("typed",data=new Typed(this,options));if(typeof option=="string")data[option]()})};$.fn.typed.defaults={strings:["These are the default values...","You know what you should do?","Use your own!","Have a great day!"],stringsElement:null,typeSpeed:0,startDelay:0,backSpeed:0,shuffle:false,backDelay:500,loop:false,loopCount:false,showCursor:true,cursorChar:"|",attr:null,contentType:"html",callback:function(){},preStringTyped:function(){},onStringTyped:function(){},resetCallback:function(){}}}(window.jQuery);

/*
* jquery-match-height 0.7.0 by @liabru
* http://brm.io/jquery-match-height/
* License MIT
*/
!function(t){"use strict";"function"==typeof define&&define.amd?define(["jquery"],t):"undefined"!=typeof module&&module.exports?module.exports=t(require("jquery")):t(jQuery)}(function(t){var e=-1,o=-1,i=function(t){return parseFloat(t)||0},a=function(e){var o=1,a=t(e),n=null,r=[];return a.each(function(){var e=t(this),a=e.offset().top-i(e.css("margin-top")),s=r.length>0?r[r.length-1]:null;null===s?r.push(e):Math.floor(Math.abs(n-a))<=o?r[r.length-1]=s.add(e):r.push(e),n=a}),r},n=function(e){var o={
byRow:!0,property:"height",target:null,remove:!1};return"object"==typeof e?t.extend(o,e):("boolean"==typeof e?o.byRow=e:"remove"===e&&(o.remove=!0),o)},r=t.fn.matchHeight=function(e){var o=n(e);if(o.remove){var i=this;return this.css(o.property,""),t.each(r._groups,function(t,e){e.elements=e.elements.not(i)}),this}return this.length<=1&&!o.target?this:(r._groups.push({elements:this,options:o}),r._apply(this,o),this)};r.version="0.7.0",r._groups=[],r._throttle=80,r._maintainScroll=!1,r._beforeUpdate=null,
r._afterUpdate=null,r._rows=a,r._parse=i,r._parseOptions=n,r._apply=function(e,o){var s=n(o),h=t(e),l=[h],c=t(window).scrollTop(),p=t("html").outerHeight(!0),d=h.parents().filter(":hidden");return d.each(function(){var e=t(this);e.data("style-cache",e.attr("style"))}),d.css("display","block"),s.byRow&&!s.target&&(h.each(function(){var e=t(this),o=e.css("display");"inline-block"!==o&&"flex"!==o&&"inline-flex"!==o&&(o="block"),e.data("style-cache",e.attr("style")),e.css({display:o,"padding-top":"0",
"padding-bottom":"0","margin-top":"0","margin-bottom":"0","border-top-width":"0","border-bottom-width":"0",height:"100px",overflow:"hidden"})}),l=a(h),h.each(function(){var e=t(this);e.attr("style",e.data("style-cache")||"")})),t.each(l,function(e,o){var a=t(o),n=0;if(s.target)n=s.target.outerHeight(!1);else{if(s.byRow&&a.length<=1)return void a.css(s.property,"");a.each(function(){var e=t(this),o=e.attr("style"),i=e.css("display");"inline-block"!==i&&"flex"!==i&&"inline-flex"!==i&&(i="block");var a={
display:i};a[s.property]="",e.css(a),e.outerHeight(!1)>n&&(n=e.outerHeight(!1)),o?e.attr("style",o):e.css("display","")})}a.each(function(){var e=t(this),o=0;s.target&&e.is(s.target)||("border-box"!==e.css("box-sizing")&&(o+=i(e.css("border-top-width"))+i(e.css("border-bottom-width")),o+=i(e.css("padding-top"))+i(e.css("padding-bottom"))),e.css(s.property,n-o+"px"))})}),d.each(function(){var e=t(this);e.attr("style",e.data("style-cache")||null)}),r._maintainScroll&&t(window).scrollTop(c/p*t("html").outerHeight(!0)),
this},r._applyDataApi=function(){var e={};t("[data-match-height], [data-mh]").each(function(){var o=t(this),i=o.attr("data-mh")||o.attr("data-match-height");i in e?e[i]=e[i].add(o):e[i]=o}),t.each(e,function(){this.matchHeight(!0)})};var s=function(e){r._beforeUpdate&&r._beforeUpdate(e,r._groups),t.each(r._groups,function(){r._apply(this.elements,this.options)}),r._afterUpdate&&r._afterUpdate(e,r._groups)};r._update=function(i,a){if(a&&"resize"===a.type){var n=t(window).width();if(n===e)return;e=n;
}i?-1===o&&(o=setTimeout(function(){s(a),o=-1},r._throttle)):s(a)},t(r._applyDataApi),t(window).bind("load",function(t){r._update(!1,t)}),t(window).bind("resize orientationchange",function(t){r._update(!0,t)})});

/*!
 * Flickity PACKAGED v1.0.0
 * Touch, responsive, flickable galleries
 *
 * Licensed GPLv3 for open source use
 * or Flickity Commercial License for commercial use
 *
 * http://flickity.metafizzy.co
 * Copyright 2015 Metafizzy
 */

!function(t){function e(){}function i(t){function i(e){e.prototype.option||(e.prototype.option=function(e){t.isPlainObject(e)&&(this.options=t.extend(!0,this.options,e))})}function o(e,i){t.fn[e]=function(o){if("string"==typeof o){for(var s=n.call(arguments,1),a=0,l=this.length;l>a;a++){var h=this[a],c=t.data(h,e);if(c)if(t.isFunction(c[o])&&"_"!==o.charAt(0)){var d=c[o].apply(c,s);if(void 0!==d)return d}else r("no such method '"+o+"' for "+e+" instance");else r("cannot call methods on "+e+" prior to initialization; attempted to call '"+o+"'")}return this}return this.each(function(){var n=t.data(this,e);n?(n.option(o),n._init()):(n=new i(this,o),t.data(this,e,n))})}}if(t){var r="undefined"==typeof console?e:function(t){console.error(t)};return t.bridget=function(t,e){i(e),o(t,e)},t.bridget}}var n=Array.prototype.slice;"function"==typeof define&&define.amd?define("jquery-bridget/jquery.bridget",["jquery"],i):i("object"==typeof exports?require("jquery"):t.jQuery)}(window),function(t){function e(t){return new RegExp("(^|\\s+)"+t+"(\\s+|$)")}function i(t,e){var i=n(t,e)?r:o;i(t,e)}var n,o,r;"classList"in document.documentElement?(n=function(t,e){return t.classList.contains(e)},o=function(t,e){t.classList.add(e)},r=function(t,e){t.classList.remove(e)}):(n=function(t,i){return e(i).test(t.className)},o=function(t,e){n(t,e)||(t.className=t.className+" "+e)},r=function(t,i){t.className=t.className.replace(e(i)," ")});var s={hasClass:n,addClass:o,removeClass:r,toggleClass:i,has:n,add:o,remove:r,toggle:i};"function"==typeof define&&define.amd?define("classie/classie",s):"object"==typeof exports?module.exports=s:t.classie=s}(window),function(){function t(){}function e(t,e){for(var i=t.length;i--;)if(t[i].listener===e)return i;return-1}function i(t){return function(){return this[t].apply(this,arguments)}}var n=t.prototype,o=this,r=o.EventEmitter;n.getListeners=function(t){var e,i,n=this._getEvents();if(t instanceof RegExp){e={};for(i in n)n.hasOwnProperty(i)&&t.test(i)&&(e[i]=n[i])}else e=n[t]||(n[t]=[]);return e},n.flattenListeners=function(t){var e,i=[];for(e=0;e<t.length;e+=1)i.push(t[e].listener);return i},n.getListenersAsObject=function(t){var e,i=this.getListeners(t);return i instanceof Array&&(e={},e[t]=i),e||i},n.addListener=function(t,i){var n,o=this.getListenersAsObject(t),r="object"==typeof i;for(n in o)o.hasOwnProperty(n)&&-1===e(o[n],i)&&o[n].push(r?i:{listener:i,once:!1});return this},n.on=i("addListener"),n.addOnceListener=function(t,e){return this.addListener(t,{listener:e,once:!0})},n.once=i("addOnceListener"),n.defineEvent=function(t){return this.getListeners(t),this},n.defineEvents=function(t){for(var e=0;e<t.length;e+=1)this.defineEvent(t[e]);return this},n.removeListener=function(t,i){var n,o,r=this.getListenersAsObject(t);for(o in r)r.hasOwnProperty(o)&&(n=e(r[o],i),-1!==n&&r[o].splice(n,1));return this},n.off=i("removeListener"),n.addListeners=function(t,e){return this.manipulateListeners(!1,t,e)},n.removeListeners=function(t,e){return this.manipulateListeners(!0,t,e)},n.manipulateListeners=function(t,e,i){var n,o,r=t?this.removeListener:this.addListener,s=t?this.removeListeners:this.addListeners;if("object"!=typeof e||e instanceof RegExp)for(n=i.length;n--;)r.call(this,e,i[n]);else for(n in e)e.hasOwnProperty(n)&&(o=e[n])&&("function"==typeof o?r.call(this,n,o):s.call(this,n,o));return this},n.removeEvent=function(t){var e,i=typeof t,n=this._getEvents();if("string"===i)delete n[t];else if(t instanceof RegExp)for(e in n)n.hasOwnProperty(e)&&t.test(e)&&delete n[e];else delete this._events;return this},n.removeAllListeners=i("removeEvent"),n.emitEvent=function(t,e){var i,n,o,r,s=this.getListenersAsObject(t);for(o in s)if(s.hasOwnProperty(o))for(n=s[o].length;n--;)i=s[o][n],i.once===!0&&this.removeListener(t,i.listener),r=i.listener.apply(this,e||[]),r===this._getOnceReturnValue()&&this.removeListener(t,i.listener);return this},n.trigger=i("emitEvent"),n.emit=function(t){var e=Array.prototype.slice.call(arguments,1);return this.emitEvent(t,e)},n.setOnceReturnValue=function(t){return this._onceReturnValue=t,this},n._getOnceReturnValue=function(){return this.hasOwnProperty("_onceReturnValue")?this._onceReturnValue:!0},n._getEvents=function(){return this._events||(this._events={})},t.noConflict=function(){return o.EventEmitter=r,t},"function"==typeof define&&define.amd?define("eventEmitter/EventEmitter",[],function(){return t}):"object"==typeof module&&module.exports?module.exports=t:o.EventEmitter=t}.call(this),function(t){function e(e){var i=t.event;return i.target=i.target||i.srcElement||e,i}var i=document.documentElement,n=function(){};i.addEventListener?n=function(t,e,i){t.addEventListener(e,i,!1)}:i.attachEvent&&(n=function(t,i,n){t[i+n]=n.handleEvent?function(){var i=e(t);n.handleEvent.call(n,i)}:function(){var i=e(t);n.call(t,i)},t.attachEvent("on"+i,t[i+n])});var o=function(){};i.removeEventListener?o=function(t,e,i){t.removeEventListener(e,i,!1)}:i.detachEvent&&(o=function(t,e,i){t.detachEvent("on"+e,t[e+i]);try{delete t[e+i]}catch(n){t[e+i]=void 0}});var r={bind:n,unbind:o};"function"==typeof define&&define.amd?define("eventie/eventie",r):"object"==typeof exports?module.exports=r:t.eventie=r}(window),function(t){function e(t){if(t){if("string"==typeof n[t])return t;t=t.charAt(0).toUpperCase()+t.slice(1);for(var e,o=0,r=i.length;r>o;o++)if(e=i[o]+t,"string"==typeof n[e])return e}}var i="Webkit Moz ms Ms O".split(" "),n=document.documentElement.style;"function"==typeof define&&define.amd?define("get-style-property/get-style-property",[],function(){return e}):"object"==typeof exports?module.exports=e:t.getStyleProperty=e}(window),function(t){function e(t){var e=parseFloat(t),i=-1===t.indexOf("%")&&!isNaN(e);return i&&e}function i(){}function n(){for(var t={width:0,height:0,innerWidth:0,innerHeight:0,outerWidth:0,outerHeight:0},e=0,i=s.length;i>e;e++){var n=s[e];t[n]=0}return t}function o(i){function o(){if(!p){p=!0;var n=t.getComputedStyle;if(h=function(){var t=n?function(t){return n(t,null)}:function(t){return t.currentStyle};return function(e){var i=t(e);return i||r("Style returned "+i+". Are you running this code in a hidden iframe on Firefox? See http://bit.ly/getsizebug1"),i}}(),c=i("boxSizing")){var o=document.createElement("div");o.style.width="200px",o.style.padding="1px 2px 3px 4px",o.style.borderStyle="solid",o.style.borderWidth="1px 2px 3px 4px",o.style[c]="border-box";var s=document.body||document.documentElement;s.appendChild(o);var a=h(o);d=200===e(a.width),s.removeChild(o)}}}function a(t){if(o(),"string"==typeof t&&(t=document.querySelector(t)),t&&"object"==typeof t&&t.nodeType){var i=h(t);if("none"===i.display)return n();var r={};r.width=t.offsetWidth,r.height=t.offsetHeight;for(var a=r.isBorderBox=!(!c||!i[c]||"border-box"!==i[c]),p=0,u=s.length;u>p;p++){var f=s[p],v=i[f];v=l(t,v);var y=parseFloat(v);r[f]=isNaN(y)?0:y}var g=r.paddingLeft+r.paddingRight,m=r.paddingTop+r.paddingBottom,b=r.marginLeft+r.marginRight,x=r.marginTop+r.marginBottom,S=r.borderLeftWidth+r.borderRightWidth,C=r.borderTopWidth+r.borderBottomWidth,w=a&&d,E=e(i.width);E!==!1&&(r.width=E+(w?0:g+S));var P=e(i.height);return P!==!1&&(r.height=P+(w?0:m+C)),r.innerWidth=r.width-(g+S),r.innerHeight=r.height-(m+C),r.outerWidth=r.width+b,r.outerHeight=r.height+x,r}}function l(e,i){if(t.getComputedStyle||-1===i.indexOf("%"))return i;var n=e.style,o=n.left,r=e.runtimeStyle,s=r&&r.left;return s&&(r.left=e.currentStyle.left),n.left=i,i=n.pixelLeft,n.left=o,s&&(r.left=s),i}var h,c,d,p=!1;return a}var r="undefined"==typeof console?i:function(t){console.error(t)},s=["paddingLeft","paddingRight","paddingTop","paddingBottom","marginLeft","marginRight","marginTop","marginBottom","borderLeftWidth","borderRightWidth","borderTopWidth","borderBottomWidth"];"function"==typeof define&&define.amd?define("get-size/get-size",["get-style-property/get-style-property"],o):"object"==typeof exports?module.exports=o(require("desandro-get-style-property")):t.getSize=o(t.getStyleProperty)}(window),function(t){function e(t){"function"==typeof t&&(e.isReady?t():s.push(t))}function i(t){var i="readystatechange"===t.type&&"complete"!==r.readyState;e.isReady||i||n()}function n(){e.isReady=!0;for(var t=0,i=s.length;i>t;t++){var n=s[t];n()}}function o(o){return"complete"===r.readyState?n():(o.bind(r,"DOMContentLoaded",i),o.bind(r,"readystatechange",i),o.bind(t,"load",i)),e}var r=t.document,s=[];e.isReady=!1,"function"==typeof define&&define.amd?define("doc-ready/doc-ready",["eventie/eventie"],o):"object"==typeof exports?module.exports=o(require("eventie")):t.docReady=o(t.eventie)}(window),function(t){function e(t,e){return t[s](e)}function i(t){if(!t.parentNode){var e=document.createDocumentFragment();e.appendChild(t)}}function n(t,e){i(t);for(var n=t.parentNode.querySelectorAll(e),o=0,r=n.length;r>o;o++)if(n[o]===t)return!0;return!1}function o(t,n){return i(t),e(t,n)}var r,s=function(){if(t.matchesSelector)return"matchesSelector";for(var e=["webkit","moz","ms","o"],i=0,n=e.length;n>i;i++){var o=e[i],r=o+"MatchesSelector";if(t[r])return r}}();if(s){var a=document.createElement("div"),l=e(a,"div");r=l?e:o}else r=n;"function"==typeof define&&define.amd?define("matches-selector/matches-selector",[],function(){return r}):"object"==typeof exports?module.exports=r:window.matchesSelector=r}(Element.prototype),function(t,e){"function"==typeof define&&define.amd?define("fizzy-ui-utils/utils",["doc-ready/doc-ready","matches-selector/matches-selector"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("doc-ready"),require("desandro-matches-selector")):t.fizzyUIUtils=e(t,t.docReady,t.matchesSelector)}(window,function(t,e,i){function n(t){return t.replace(/(.)([A-Z])/g,function(t,e,i){return e+"-"+i}).toLowerCase()}var o={};o.extend=function(t,e){for(var i in e)t[i]=e[i];return t},o.modulo=function(t,e){return(t%e+e)%e};var r=Object.prototype.toString;o.isArray=function(t){return"[object Array]"==r.call(t)},o.makeArray=function(t){var e=[];if(o.isArray(t))e=t;else if(t&&"number"==typeof t.length)for(var i=0,n=t.length;n>i;i++)e.push(t[i]);else e.push(t);return e},o.indexOf=Array.prototype.indexOf?function(t,e){return t.indexOf(e)}:function(t,e){for(var i=0,n=t.length;n>i;i++)if(t[i]===e)return i;return-1},o.removeFrom=function(t,e){var i=o.indexOf(t,e);-1!=i&&t.splice(i,1)},o.isElement="function"==typeof HTMLElement||"object"==typeof HTMLElement?function(t){return t instanceof HTMLElement}:function(t){return t&&"object"==typeof t&&1==t.nodeType&&"string"==typeof t.nodeName},o.setText=function(){function t(t,i){e=e||(void 0!==document.documentElement.textContent?"textContent":"innerText"),t[e]=i}var e;return t}(),o.getParent=function(t,e){for(;t!=document.body;)if(t=t.parentNode,i(t,e))return t},o.getQueryElement=function(t){return"string"==typeof t?document.querySelector(t):t},o.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},o.filterFindElements=function(t,e){t=o.makeArray(t);for(var n=[],r=0,s=t.length;s>r;r++){var a=t[r];if(o.isElement(a))if(e){i(a,e)&&n.push(a);for(var l=a.querySelectorAll(e),h=0,c=l.length;c>h;h++)n.push(l[h])}else n.push(a)}return n},o.debounceMethod=function(t,e,i){var n=t.prototype[e],o=e+"Timeout";t.prototype[e]=function(){var t=this[o];t&&clearTimeout(t);var e=arguments,r=this;this[o]=setTimeout(function(){n.apply(r,e),delete r[o]},i||100)}};var s=t.jQuery,a=t.console;return o.htmlInit=function(t,i){e(function(){for(var e=n(i),o=document.querySelectorAll(".js-"+e),r="data-"+e+"-options",l=0,h=o.length;h>l;l++){var c,d=o[l],p=d.getAttribute(r);try{c=p&&JSON.parse(p)}catch(u){a&&a.error("Error parsing "+r+" on "+d.nodeName.toLowerCase()+(d.id?"#"+d.id:"")+": "+u);continue}var f=new t(d,c);s&&s.data(d,i,f)}})},o}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/cell",["get-size/get-size"],function(i){return e(t,i)}):"object"==typeof exports?module.exports=e(t,require("get-size")):(t.Flickity=t.Flickity||{},t.Flickity.Cell=e(t,t.getSize))}(window,function(t,e){function i(t,e){this.element=t,this.parent=e,this.create()}var n="attachEvent"in t;return i.prototype.create=function(){this.element.style.position="absolute",n&&this.element.setAttribute("unselectable","on"),this.x=0,this.shift=0},i.prototype.destroy=function(){this.element.style.position="";var t=this.parent.originSide;this.element.style[t]=""},i.prototype.getSize=function(){this.size=e(this.element)},i.prototype.setPosition=function(t){this.x=t,this.setDefaultTarget(),this.renderPosition(t)},i.prototype.setDefaultTarget=function(){var t="left"==this.parent.originSide?"marginLeft":"marginRight";this.target=this.x+this.size[t]+this.size.width*this.parent.cellAlign},i.prototype.renderPosition=function(t){var e=this.parent.originSide;this.element.style[e]=this.parent.getPositionValue(t)},i.prototype.wrapShift=function(t){this.shift=t,this.renderPosition(this.x+this.parent.slideableWidth*t)},i.prototype.remove=function(){this.element.parentNode.removeChild(this.element)},i}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/animate",["get-style-property/get-style-property","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("desandro-get-style-property"),require("fizzy-ui-utils")):(t.Flickity=t.Flickity||{},t.Flickity.animatePrototype=e(t,t.getStyleProperty,t.fizzyUIUtils))}(window,function(t,e,i){for(var n,o=0,r="webkit moz ms o".split(" "),s=t.requestAnimationFrame,a=t.cancelAnimationFrame,l=0;l<r.length&&(!s||!a);l++)n=r[l],s=s||t[n+"RequestAnimationFrame"],a=a||t[n+"CancelAnimationFrame"]||t[n+"CancelRequestAnimationFrame"];s&&a||(s=function(e){var i=(new Date).getTime(),n=Math.max(0,16-(i-o)),r=t.setTimeout(function(){e(i+n)},n);return o=i+n,r},a=function(e){t.clearTimeout(e)});var h={};h.startAnimation=function(){this.isAnimating||(this.isAnimating=!0,this.restingFrames=0,this.animate())},h.animate=function(){this.applySelectedAttraction();var t=this.x;if(this.integratePhysics(),this.positionSlider(),this.settle(t),this.isAnimating){var e=this;s(function(){e.animate()})}};var c=e("transform"),d=!!e("perspective");return h.positionSlider=function(){var t=this.x;this.options.wrapAround&&this.cells.length>1&&(t=i.modulo(t,this.slideableWidth),t-=this.slideableWidth,this.shiftWrapCells(t)),t+=this.cursorPosition,t=this.options.rightToLeft&&c?-t:t;var e=this.getPositionValue(t);c?this.slider.style[c]=d&&this.isAnimating?"translate3d("+e+",0,0)":"translateX("+e+")":this.slider.style[this.originSide]=e},h.positionSliderAtSelected=function(){if(this.cells.length){var t=this.cells[this.selectedIndex];this.x=-t.target,this.positionSlider()}},h.getPositionValue=function(t){return this.options.percentPosition?.01*Math.round(t/this.size.innerWidth*1e4)+"%":Math.round(t)+"px"},h.settle=function(t){this.isPointerDown||Math.round(100*this.x)!=Math.round(100*t)||this.restingFrames++,this.restingFrames>2&&(this.isAnimating=!1,delete this.isFreeScrolling,d&&this.positionSlider(),this.dispatchEvent("settle"))},h.shiftWrapCells=function(t){var e=this.cursorPosition+t;this._shiftCells(this.beforeShiftCells,e,-1);var i=this.size.innerWidth-(t+this.slideableWidth+this.cursorPosition);this._shiftCells(this.afterShiftCells,i,1)},h._shiftCells=function(t,e,i){for(var n=0,o=t.length;o>n;n++){var r=t[n],s=e>0?i:0;r.wrapShift(s),e-=r.size.outerWidth}},h._unshiftCells=function(t){if(t&&t.length)for(var e=0,i=t.length;i>e;e++)t[e].wrapShift(0)},h.integratePhysics=function(){this.velocity+=this.accel,this.x+=this.velocity,this.velocity*=this.getFrictionFactor(),this.accel=0},h.applyForce=function(t){this.accel+=t},h.getFrictionFactor=function(){return 1-this.options[this.isFreeScrolling?"freeScrollFriction":"friction"]},h.getRestingPosition=function(){return this.x+this.velocity/(1-this.getFrictionFactor())},h.applySelectedAttraction=function(){var t=this.cells.length;if(!this.isPointerDown&&!this.isFreeScrolling&&t){var e=this.cells[this.selectedIndex],i=this.options.wrapAround&&t>1?this.slideableWidth*Math.floor(this.selectedIndex/t):0,n=-1*(e.target+i)-this.x,o=n*this.options.selectedAttraction;this.applyForce(o)}},h}),function(t,e){if("function"==typeof define&&define.amd)define("flickity/js/flickity",["classie/classie","eventEmitter/EventEmitter","eventie/eventie","get-size/get-size","fizzy-ui-utils/utils","./cell","./animate"],function(i,n,o,r,s,a,l){return e(t,i,n,o,r,s,a,l)});else if("object"==typeof exports)module.exports=e(t,require("desandro-classie"),require("wolfy87-eventemitter"),require("eventie"),require("get-size"),require("fizzy-ui-utils"),require("./cell"),require("./animate"));else{var i=t.Flickity;t.Flickity=e(t,t.classie,t.EventEmitter,t.eventie,t.getSize,t.fizzyUIUtils,i.Cell,i.animatePrototype)}}(window,function(t,e,i,n,o,r,s,a){function l(t,e){for(t=r.makeArray(t);t.length;)e.appendChild(t.shift())}function h(t,e){var i=r.getQueryElement(t);return i?(this.element=i,c&&(this.$element=c(this.element)),this.options=r.extend({},this.constructor.defaults),this.option(e),void this._create()):void(p&&p.error("Bad element for Flickity: "+(i||t)))}var c=t.jQuery,d=t.getComputedStyle,p=t.console,u=0,f={};h.defaults={accessibility:!0,cellAlign:"center",freeScrollFriction:.075,friction:.28,percentPosition:!0,resize:!0,selectedAttraction:.025,setGallerySize:!0},h.createMethods=[],r.extend(h.prototype,i.prototype),h.prototype._create=function(){var e=this.guid=++u;this.element.flickityGUID=e,f[e]=this,this.selectedIndex=this.options.initialIndex||0,this.restingFrames=0,this.x=0,this.velocity=0,this.accel=0,this.originSide=this.options.rightToLeft?"right":"left",this.viewport=document.createElement("div"),this.viewport.className="flickity-viewport",h.setUnselectable(this.viewport),this._createSlider(),(this.options.resize||this.options.watchCSS)&&(n.bind(t,"resize",this),this.isResizeBound=!0);for(var i=0,o=h.createMethods.length;o>i;i++){var r=h.createMethods[i];this[r]()}this.options.watchCSS?this.watchCSS():this.activate()},h.prototype.option=function(t){r.extend(this.options,t)},h.prototype.activate=function(){if(!this.isActive){this.isActive=!0,e.add(this.element,"flickity-enabled"),this.options.rightToLeft&&e.add(this.element,"flickity-rtl");var t=this._filterFindCellElements(this.element.children);l(t,this.slider),this.viewport.appendChild(this.slider),this.element.appendChild(this.viewport),this.getSize(),this.reloadCells(),this.setGallerySize(),this.options.accessibility&&(this.element.tabIndex=0,n.bind(this.element,"keydown",this)),this.emit("activate"),this.positionSliderAtSelected(),this.select(this.selectedIndex)}},h.prototype._createSlider=function(){var t=document.createElement("div");t.className="flickity-slider",t.style[this.originSide]=0,this.slider=t},h.prototype._filterFindCellElements=function(t){return r.filterFindElements(t,this.options.cellSelector)},h.prototype.reloadCells=function(){this.cells=this._makeCells(this.slider.children),this.positionCells(),this._getWrapShiftCells(),this.setGallerySize()},h.prototype._makeCells=function(t){for(var e=this._filterFindCellElements(t),i=[],n=0,o=e.length;o>n;n++){var r=e[n],a=new s(r,this);i.push(a)}return i},h.prototype.getLastCell=function(){return this.cells[this.cells.length-1]},h.prototype.positionCells=function(){this._sizeCells(this.cells),this._positionCells(0)},h.prototype._positionCells=function(t){this.maxCellHeight=t?this.maxCellHeight||0:0;var e=0;if(t>0){var i=this.cells[t-1];e=i.x+i.size.outerWidth}for(var n,o=this.cells.length,r=t;o>r;r++)n=this.cells[r],n.setPosition(e),e+=n.size.outerWidth,this.maxCellHeight=Math.max(n.size.outerHeight,this.maxCellHeight);this.slideableWidth=e,this._containCells()},h.prototype._sizeCells=function(t){for(var e=0,i=t.length;i>e;e++){var n=t[e];n.getSize()}},h.prototype._init=h.prototype.reposition=function(){this.positionCells(),this.positionSliderAtSelected()},h.prototype.getSize=function(){this.size=o(this.element),this.setCellAlign(),this.cursorPosition=this.size.innerWidth*this.cellAlign};var v={center:{left:.5,right:.5},left:{left:0,right:1},right:{right:0,left:1}};h.prototype.setCellAlign=function(){var t=v[this.options.cellAlign];this.cellAlign=t?t[this.originSide]:this.options.cellAlign},h.prototype.setGallerySize=function(){this.options.setGallerySize&&(this.viewport.style.height=this.maxCellHeight+"px")},h.prototype._getWrapShiftCells=function(){if(this.options.wrapAround){this._unshiftCells(this.beforeShiftCells),this._unshiftCells(this.afterShiftCells);var t=this.cursorPosition,e=this.cells.length-1;this.beforeShiftCells=this._getGapCells(t,e,-1),t=this.size.innerWidth-this.cursorPosition,this.afterShiftCells=this._getGapCells(t,0,1)}},h.prototype._getGapCells=function(t,e,i){for(var n=[];t>0;){var o=this.cells[e];if(!o)break;n.push(o),e+=i,t-=o.size.outerWidth}return n},h.prototype._containCells=function(){if(this.options.contain&&!this.options.wrapAround&&this.cells.length)for(var t=this.options.rightToLeft?"marginRight":"marginLeft",e=this.options.rightToLeft?"marginLeft":"marginRight",i=this.cells[0].size[t],n=this.getLastCell(),o=this.slideableWidth-n.size[e],r=o-this.size.innerWidth*(1-this.cellAlign),s=o<this.size.innerWidth,a=0,l=this.cells.length;l>a;a++){var h=this.cells[a];h.setDefaultTarget(),s?h.target=o*this.cellAlign:(h.target=Math.max(h.target,this.cursorPosition+i),h.target=Math.min(h.target,r))}},h.prototype.dispatchEvent=function(t,e,i){var n=[e].concat(i);if(this.emitEvent(t,n),c&&this.$element)if(e){var o=c.Event(e);o.type=t,this.$element.trigger(o,i)}else this.$element.trigger(t,i)},h.prototype.select=function(t,e){if(this.isActive){var i=this.cells.length;this.options.wrapAround&&i>1&&(0>t?this.x-=this.slideableWidth:t>=i&&(this.x+=this.slideableWidth)),(this.options.wrapAround||e)&&(t=r.modulo(t,i)),this.cells[t]&&(this.selectedIndex=t,this.setSelectedCell(),this.startAnimation(),this.dispatchEvent("cellSelect"))}},h.prototype.previous=function(t){this.select(this.selectedIndex-1,t)},h.prototype.next=function(t){this.select(this.selectedIndex+1,t)},h.prototype.setSelectedCell=function(){this._removeSelectedCellClass(),this.selectedCell=this.cells[this.selectedIndex],this.selectedElement=this.selectedCell.element,e.add(this.selectedElement,"is-selected")},h.prototype._removeSelectedCellClass=function(){this.selectedCell&&e.remove(this.selectedCell.element,"is-selected")},h.prototype.getCell=function(t){for(var e=0,i=this.cells.length;i>e;e++){var n=this.cells[e];if(n.element==t)return n}},h.prototype.getCells=function(t){t=r.makeArray(t);for(var e=[],i=0,n=t.length;n>i;i++){var o=t[i],s=this.getCell(o);s&&e.push(s)}return e},h.prototype.getCellElements=function(){for(var t=[],e=0,i=this.cells.length;i>e;e++)t.push(this.cells[e].element);return t},h.prototype.getParentCell=function(t){var e=this.getCell(t);return e?e:(t=r.getParent(t,".flickity-slider > *"),this.getCell(t))},h.prototype.uiChange=function(){this.emit("uiChange")},h.prototype.childUIPointerDown=function(t){this.emitEvent("childUIPointerDown",[t])},h.prototype.onresize=function(){this.watchCSS(),this.resize()},r.debounceMethod(h,"onresize",150),h.prototype.resize=function(){this.isActive&&(this.getSize(),this.options.wrapAround&&(this.x=r.modulo(this.x,this.slideableWidth)),this.positionCells(),this._getWrapShiftCells(),this.setGallerySize(),this.positionSliderAtSelected())};var y=h.supportsConditionalCSS=function(){var t;return function(){if(void 0!==t)return t;if(!d)return void(t=!1);var e=document.createElement("style"),i=document.createTextNode('body:after { content: "foo"; display: none; }');e.appendChild(i),document.head.appendChild(e);var n=d(document.body,":after").content;return t=-1!=n.indexOf("foo"),document.head.removeChild(e),t}}();h.prototype.watchCSS=function(){var t=this.options.watchCSS;if(t){var e=y();if(!e){var i="fallbackOn"==t?"activate":"deactivate";return void this[i]()}var n=d(this.element,":after").content;-1!=n.indexOf("flickity")?this.activate():this.deactivate()}},h.prototype.onkeydown=function(t){if(this.options.accessibility&&(!document.activeElement||document.activeElement==this.element))if(37==t.keyCode){var e=this.options.rightToLeft?"next":"previous";this.uiChange(),this[e]()}else if(39==t.keyCode){var i=this.options.rightToLeft?"previous":"next";this.uiChange(),this[i]()}},h.prototype.deactivate=function(){if(this.isActive){e.remove(this.element,"flickity-enabled"),e.remove(this.element,"flickity-rtl");for(var t=0,i=this.cells.length;i>t;t++){var o=this.cells[t];o.destroy()}this._removeSelectedCellClass(),this.element.removeChild(this.viewport),l(this.slider.children,this.element),this.options.accessibility&&(this.element.removeAttribute("tabIndex"),n.unbind(this.element,"keydown",this)),this.isActive=!1,this.emit("deactivate")}},h.prototype.destroy=function(){this.deactivate(),this.isResizeBound&&n.unbind(t,"resize",this),this.emit("destroy"),c&&this.$element&&c.removeData(this.element,"flickity"),delete this.element.flickityGUID,delete f[this.guid]},r.extend(h.prototype,a);var g="attachEvent"in t;return h.setUnselectable=function(t){g&&t.setAttribute("unselectable","on")},h.data=function(t){t=r.getQueryElement(t);var e=t&&t.flickityGUID;return e&&f[e]},r.htmlInit(h,"flickity"),c&&c.bridget&&c.bridget("flickity",h),h.Cell=s,h}),function(t,e){"function"==typeof define&&define.amd?define("unipointer/unipointer",["eventEmitter/EventEmitter","eventie/eventie"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("wolfy87-eventemitter"),require("eventie")):t.Unipointer=e(t,t.EventEmitter,t.eventie)}(window,function(t,e,i){function n(){}function o(){}o.prototype=new e,o.prototype.bindStartEvent=function(t){this._bindStartEvent(t,!0)},o.prototype.unbindStartEvent=function(t){this._bindStartEvent(t,!1)},o.prototype._bindStartEvent=function(e,n){n=void 0===n?!0:!!n;var o=n?"bind":"unbind";t.navigator.pointerEnabled?i[o](e,"pointerdown",this):t.navigator.msPointerEnabled?i[o](e,"MSPointerDown",this):(i[o](e,"mousedown",this),i[o](e,"touchstart",this))},o.prototype.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},o.prototype.getTouch=function(t){for(var e=0,i=t.length;i>e;e++){var n=t[e];if(n.identifier==this.pointerIdentifier)return n}},o.prototype.onmousedown=function(t){var e=t.button;e&&0!==e&&1!==e||this._pointerDown(t,t)},o.prototype.ontouchstart=function(t){this._pointerDown(t,t.changedTouches[0])},o.prototype.onMSPointerDown=o.prototype.onpointerdown=function(t){this._pointerDown(t,t)},o.prototype._pointerDown=function(t,e){this.isPointerDown||(this.isPointerDown=!0,this.pointerIdentifier=void 0!==e.pointerId?e.pointerId:e.identifier,this.pointerDown(t,e))},o.prototype.pointerDown=function(t,e){this._bindPostStartEvents(t),this.emitEvent("pointerDown",[this,t,e])};var r={mousedown:["mousemove","mouseup"],touchstart:["touchmove","touchend","touchcancel"],pointerdown:["pointermove","pointerup","pointercancel"],MSPointerDown:["MSPointerMove","MSPointerUp","MSPointerCancel"]};return o.prototype._bindPostStartEvents=function(e){if(e){for(var n=r[e.type],o=e.preventDefault?t:document,s=0,a=n.length;a>s;s++){var l=n[s];i.bind(o,l,this)}this._boundPointerEvents={events:n,node:o}}},o.prototype._unbindPostStartEvents=function(){var t=this._boundPointerEvents;if(t&&t.events){for(var e=0,n=t.events.length;n>e;e++){var o=t.events[e];i.unbind(t.node,o,this)}delete this._boundPointerEvents}},o.prototype.onmousemove=function(t){this._pointerMove(t,t)},o.prototype.onMSPointerMove=o.prototype.onpointermove=function(t){t.pointerId==this.pointerIdentifier&&this._pointerMove(t,t)},o.prototype.ontouchmove=function(t){var e=this.getTouch(t.changedTouches);e&&this._pointerMove(t,e)},o.prototype._pointerMove=function(t,e){this.pointerMove(t,e)},o.prototype.pointerMove=function(t,e){this.emitEvent("pointerMove",[this,t,e])},o.prototype.onmouseup=function(t){this._pointerUp(t,t)},o.prototype.onMSPointerUp=o.prototype.onpointerup=function(t){t.pointerId==this.pointerIdentifier&&this._pointerUp(t,t)},o.prototype.ontouchend=function(t){var e=this.getTouch(t.changedTouches);e&&this._pointerUp(t,e)},o.prototype._pointerUp=function(t,e){this._pointerDone(),this.pointerUp(t,e)},o.prototype.pointerUp=function(t,e){this.emitEvent("pointerUp",[this,t,e])},o.prototype._pointerDone=function(){this.isPointerDown=!1,delete this.pointerIdentifier,this._unbindPostStartEvents(),this.pointerDone()},o.prototype.pointerDone=n,o.prototype.onMSPointerCancel=o.prototype.onpointercancel=function(t){t.pointerId==this.pointerIdentifier&&this._pointerCancel(t,t)},o.prototype.ontouchcancel=function(t){var e=this.getTouch(t.changedTouches);e&&this._pointerCancel(t,e)},o.prototype._pointerCancel=function(t,e){this._pointerDone(),this.pointerCancel(t,e)},o.prototype.pointerCancel=function(t,e){this.emitEvent("pointerCancel",[this,t,e])},o.getPointerPoint=function(t){return{x:void 0!==t.pageX?t.pageX:t.clientX,y:void 0!==t.pageY?t.pageY:t.clientY}},o}),function(t,e){"function"==typeof define&&define.amd?define("unidragger/unidragger",["eventie/eventie","unipointer/unipointer"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("eventie"),require("unipointer")):t.Unidragger=e(t,t.eventie,t.Unipointer)}(window,function(t,e,i){function n(){}function o(t){t.preventDefault?t.preventDefault():t.returnValue=!1}function r(t){for(;t!=document.body;)if(t=t.parentNode,"A"==t.nodeName)return t}function s(){}function a(){return!1}s.prototype=new i,s.prototype.bindHandles=function(){this._bindHandles(!0)},s.prototype.unbindHandles=function(){this._bindHandles(!1)};var l=t.navigator;s.prototype._bindHandles=function(t){t=void 0===t?!0:!!t;var i;i=l.pointerEnabled?function(e){e.style.touchAction=t?"none":""}:l.msPointerEnabled?function(e){e.style.msTouchAction=t?"none":""}:function(){t&&c(s)};for(var n=t?"bind":"unbind",o=0,r=this.handles.length;r>o;o++){var s=this.handles[o];this._bindStartEvent(s,t),i(s),e[n](s,"click",this)}};var h="attachEvent"in document.documentElement,c=h?function(t){"IMG"==t.nodeName&&(t.ondragstart=a);for(var e=t.querySelectorAll("img"),i=0,n=e.length;n>i;i++){var o=e[i];o.ondragstart=a}}:n,d=s.allowTouchstartNodes={INPUT:!0,A:!0,BUTTON:!0,SELECT:!0};return s.prototype.pointerDown=function(t,e){this._dragPointerDown(t,e);var i=document.activeElement;i&&i.blur&&i.blur(),this._bindPostStartEvents(t),this.emitEvent("pointerDown",[this,t,e])},s.prototype._dragPointerDown=function(t,e){this.pointerDownPoint=i.getPointerPoint(e);var n=t.target.nodeName,s="touchstart"==t.type&&(d[n]||r(t.target));s||"SELECT"==n||o(t)},s.prototype.pointerMove=function(t,e){var i=this._dragPointerMove(t,e);this.emitEvent("pointerMove",[this,t,e,i]),this._dragMove(t,e,i)},s.prototype._dragPointerMove=function(t,e){var n=i.getPointerPoint(e),o={x:n.x-this.pointerDownPoint.x,y:n.y-this.pointerDownPoint.y};return!this.isDragging&&this.hasDragStarted(o)&&this._dragStart(t,e),o},s.prototype.hasDragStarted=function(t){return Math.abs(t.x)>3||Math.abs(t.y)>3},s.prototype.pointerUp=function(t,e){this.emitEvent("pointerUp",[this,t,e]),this._dragPointerUp(t,e)},s.prototype._dragPointerUp=function(t,e){this.isDragging?this._dragEnd(t,e):this._staticClick(t,e)},s.prototype._dragStart=function(t,e){this.isDragging=!0,this.dragStartPoint=s.getPointerPoint(e),this.isPreventingClicks=!0,this.dragStart(t,e)},s.prototype.dragStart=function(t,e){this.emitEvent("dragStart",[this,t,e])},s.prototype._dragMove=function(t,e,i){this.isDragging&&this.dragMove(t,e,i)},s.prototype.dragMove=function(t,e,i){this.emitEvent("dragMove",[this,t,e,i])},s.prototype._dragEnd=function(t,e){this.isDragging=!1;var i=this;setTimeout(function(){delete i.isPreventingClicks}),this.dragEnd(t,e)},s.prototype.dragEnd=function(t,e){this.emitEvent("dragEnd",[this,t,e])},s.prototype.onclick=function(t){this.isPreventingClicks&&o(t)},s.prototype._staticClick=function(t,e){"INPUT"==t.target.nodeName&&"text"==t.target.type&&t.target.focus(),this.staticClick(t,e)
},s.prototype.staticClick=function(t,e){this.emitEvent("staticClick",[this,t,e])},s.getPointerPoint=function(t){return{x:void 0!==t.pageX?t.pageX:t.clientX,y:void 0!==t.pageY?t.pageY:t.clientY}},s.getPointerPoint=i.getPointerPoint,s}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/drag",["classie/classie","eventie/eventie","./flickity","unidragger/unidragger","fizzy-ui-utils/utils"],function(i,n,o,r,s){return e(t,i,n,o,r,s)}):"object"==typeof exports?module.exports=e(t,require("desandro-classie"),require("eventie"),require("./flickity"),require("unidragger"),require("fizzy-ui-utils")):(t.Flickity=t.Flickity||{},t.Flickity.dragPrototype=e(t,t.classie,t.eventie,t.Flickity,t.Unidragger,t.fizzyUIUtils))}(window,function(t,e,i,n,o,r){function s(t){t.preventDefault?t.preventDefault():t.returnValue=!1}function a(e){var i=o.getPointerPoint(e);return i.y-t.pageYOffset}r.extend(n.defaults,{draggable:!0,touchVerticalScroll:!0}),n.createMethods.push("_createDrag");var l={};r.extend(l,o.prototype),l._createDrag=function(){this.on("activate",this.bindDrag),this.on("uiChange",this._uiChangeDrag),this.on("childUIPointerDown",this._childUIPointerDownDrag),this.on("deactivate",this.unbindDrag)},l.bindDrag=function(){this.options.draggable&&!this.isDragBound&&(e.add(this.element,"is-draggable"),this.handles=[this.viewport],this.bindHandles(),this.isDragBound=!0)},l.unbindDrag=function(){this.isDragBound&&(e.remove(this.element,"is-draggable"),this.unbindHandles(),delete this.isDragBound)},l.hasDragStarted=function(t){return Math.abs(t.x)>3},l._uiChangeDrag=function(){delete this.isFreeScrolling},l._childUIPointerDownDrag=function(t){s(t),this.pointerDownFocus(t)},l.pointerDown=function(t,i){this._dragPointerDown(t,i);var n=document.activeElement;n&&n.blur&&n!=this.element&&n.blur(),this.pointerDownFocus(t),this.velocity=0,e.add(this.viewport,"is-pointer-down"),this._bindPostStartEvents(t),this.dispatchEvent("pointerDown",t,[i])};var h={touchstart:!0,MSPointerDown:!0},c={INPUT:!0,SELECT:!0};l.pointerDownFocus=function(t){!this.options.accessibility||h[t.type]||c[t.target.nodeName]||this.element.focus()},l.pointerMove=function(t,e){var i=this._dragPointerMove(t,e);this.touchVerticalScrollMove(t,e,i),this._dragMove(t,e,i),this.dispatchEvent("pointerMove",t,[e,i])},l.pointerUp=function(t,i){delete this.isTouchScrolling,e.remove(this.viewport,"is-pointer-down"),this.dispatchEvent("pointerUp",t,[i]),this._dragPointerUp(t,i)};var d={touchmove:!0,MSPointerMove:!0};return l.touchVerticalScrollMove=function(e,i,n){if(this.options.touchVerticalScroll&&d[e.type]&&(!this.isTouchScrolling&&Math.abs(n.y)>16&&(this.startScrollY=t.pageYOffset,this.pointerWindowStartY=a(i),this.isTouchScrolling=!0),this.isTouchScrolling)){var o=this.pointerWindowStartY-a(i),r=this.startScrollY+o;t.scroll(t.pageXOffset,r)}},l.dragStart=function(t,e){this.dragStartPosition=this.x,this.startAnimation(),this.dispatchEvent("dragStart",t,[e])},l.dragMove=function(t,e,i){this.previousDragX=this.x;var n=i.x,o=this.options.rightToLeft?-1:1;if(this.x=this.dragStartPosition+n*o,!this.options.wrapAround&&this.cells.length){var r=Math.max(-this.cells[0].target,this.dragStartPosition);this.x=this.x>r?.5*(this.x-r)+r:this.x;var s=Math.min(-this.getLastCell().target,this.dragStartPosition);this.x=this.x<s?.5*(this.x-s)+s:this.x}this.previousDragMoveTime=this.dragMoveTime,this.dragMoveTime=new Date,this.dispatchEvent("dragMove",t,[e,i])},l.dragEnd=function(t,e){this.dragEndFlick(),this.options.freeScroll&&(this.isFreeScrolling=!0);var i=this.dragEndRestingSelect();if(this.options.freeScroll&&!this.options.wrapAround){var n=this.getRestingPosition();this.isFreeScrolling=-n>this.cells[0].target&&-n<this.getLastCell().target}else this.options.freeScroll||i!=this.selectedIndex||(i+=this.dragEndBoostSelect());this.select(i),this.dispatchEvent("dragEnd",t,[e])},l.dragEndFlick=function(){if(isFinite(this.previousDragX)){var t=this.dragMoveTime-this.previousDragMoveTime;if(t){t/=1e3/60;var e=this.x-this.previousDragX;this.velocity=e/t}delete this.previousDragX}},l.dragEndRestingSelect=function(){var t=this.getRestingPosition(),e=Math.abs(this.getCellDistance(-t,this.selectedIndex)),i=this._getClosestResting(t,e,1),n=this._getClosestResting(t,e,-1),o=i.distance<n.distance?i.index:n.index;return this.options.contain&&!this.options.wrapAround&&(o=Math.abs(o-this.selectedIndex)<=1?this.selectedIndex:o),o},l._getClosestResting=function(t,e,i){for(var n=this.selectedIndex,o=1/0,r=this.options.contain&&!this.options.wrapAround?function(t,e){return e>=t}:function(t,e){return e>t};r(e,o)&&(n+=i,o=e,e=this.getCellDistance(-t,n),null!==e);)e=Math.abs(e);return{distance:o,index:n-i}},l.getCellDistance=function(t,e){var i=this.cells.length,n=this.options.wrapAround&&i>1,o=n?r.modulo(e,i):e,s=this.cells[o];if(!s)return null;var a=n?this.slideableWidth*Math.floor(e/i):0;return t-(s.target+a)},l.dragEndBoostSelect=function(){var t=this.getCellDistance(-this.x,this.selectedIndex);return t>0&&this.velocity<-1?1:0>t&&this.velocity>1?-1:0},l.staticClick=function(t,e){var i=this.getParentCell(t.target),n=i&&i.element,o=i&&r.indexOf(this.cells,i);this.dispatchEvent("staticClick",t,[e,n,o])},r.extend(n.prototype,l),n}),function(t,e){"function"==typeof define&&define.amd?define("tap-listener/tap-listener",["unipointer/unipointer"],function(i){return e(t,i)}):"object"==typeof exports?module.exports=e(t,require("unipointer")):t.TapListener=e(t,t.Unipointer)}(window,function(t,e){function i(t){this.bindTap(t)}i.prototype=new e,i.prototype.bindTap=function(t){t&&(this.unbindTap(),this.tapElement=t,this._bindStartEvent(t,!0))},i.prototype.unbindTap=function(){this.tapElement&&(this._bindStartEvent(this.tapElement,!0),delete this.tapElement)};var n=void 0!==t.pageYOffset;return i.prototype.pointerUp=function(i,o){var r=e.getPointerPoint(o),s=this.tapElement.getBoundingClientRect(),a=n?t.pageXOffset:document.body.scrollLeft,l=n?t.pageYOffset:document.body.scrollTop,h=r.x>=s.left+a&&r.x<=s.right+a&&r.y>=s.top+l&&r.y<=s.bottom+l;h&&this.emitEvent("tap",[this,i,o])},i.prototype.destroy=function(){this.pointerDone(),this.unbindTap()},i}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/prev-next-button",["eventie/eventie","./flickity","tap-listener/tap-listener","fizzy-ui-utils/utils"],function(i,n,o,r){return e(t,i,n,o,r)}):"object"==typeof exports?module.exports=e(t,require("eventie"),require("./flickity"),require("tap-listener"),require("fizzy-ui-utils")):(t.Flickity=t.Flickity||{},t.Flickity.PrevNextButton=e(t,t.eventie,t.Flickity,t.TapListener,t.fizzyUIUtils))}(window,function(t,e,i,n,o){function r(t,e){this.direction=t,this.parent=e,this._create()}var s="http://www.w3.org/2000/svg",a=function(){function t(){if(void 0!==e)return e;var t=document.createElement("div");return t.innerHTML="<svg/>",e=(t.firstChild&&t.firstChild.namespaceURI)==s}var e;return t}();return r.prototype=new n,r.prototype._create=function(){this.isEnabled=!0,this.isPrevious=-1==this.direction;var t=this.parent.options.rightToLeft?1:-1;this.isLeft=this.direction==t;var e=this.element=document.createElement("button");if(e.className="flickity-prev-next-button",e.className+=this.isPrevious?" previous":" next",e.setAttribute("type","button"),i.setUnselectable(e),a()){var n=this.createSVG();e.appendChild(n)}else this.setArrowText(),e.className+=" no-svg";var o=this;this.onCellSelect=function(){o.update()},this.parent.on("cellSelect",this.onCellSelect),this.on("tap",this.onTap),this.on("pointerDown",function(t,e){o.parent.childUIPointerDown(e)})},r.prototype.activate=function(){this.update(),this.bindTap(this.element),e.bind(this.element,"click",this),this.parent.element.appendChild(this.element)},r.prototype.deactivate=function(){this.parent.element.removeChild(this.element),n.prototype.destroy.call(this),e.unbind(this.element,"click",this)},r.prototype.createSVG=function(){var t=document.createElementNS(s,"svg");t.setAttribute("viewBox","0 0 100 100");var e=document.createElementNS(s,"path");e.setAttribute("d","M 50,0 L 60,10 L 20,50 L 60,90 L 50,100 L 0,50 Z"),e.setAttribute("class","arrow");var i=this.isLeft?"translate(15,0)":"translate(85,100) rotate(180)";return e.setAttribute("transform",i),t.appendChild(e),t},r.prototype.setArrowText=function(){var t=this.parent.options,e=this.isLeft?t.leftArrowText:t.rightArrowText;o.setText(this.element,e)},r.prototype.onTap=function(){if(this.isEnabled){this.parent.uiChange();var t=this.isPrevious?"previous":"next";this.parent[t]()}},r.prototype.handleEvent=o.handleEvent,r.prototype.onclick=function(){var t=document.activeElement;t&&t==this.element&&this.onTap()},r.prototype.enable=function(){this.isEnabled||(this.element.disabled=!1,this.isEnabled=!0)},r.prototype.disable=function(){this.isEnabled&&(this.element.disabled=!0,this.isEnabled=!1)},r.prototype.update=function(){var t=this.parent.cells;if(this.parent.options.wrapAround&&t.length>1)return void this.enable();var e=t.length?t.length-1:0,i=this.isPrevious?0:e,n=this.parent.selectedIndex==i?"disable":"enable";this[n]()},r.prototype.destroy=function(){this.deactivate()},o.extend(i.defaults,{prevNextButtons:!0,leftArrowText:"‹",rightArrowText:"›"}),i.createMethods.push("_createPrevNextButtons"),i.prototype._createPrevNextButtons=function(){this.options.prevNextButtons&&(this.prevButton=new r(-1,this),this.nextButton=new r(1,this),this.on("activate",this.activatePrevNextButtons))},i.prototype.activatePrevNextButtons=function(){this.prevButton.activate(),this.nextButton.activate(),this.on("deactivate",this.deactivatePrevNextButtons)},i.prototype.deactivatePrevNextButtons=function(){this.prevButton.deactivate(),this.nextButton.deactivate(),this.off("deactivate",this.deactivatePrevNextButtons)},i.PrevNextButton=r,r}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/page-dots",["eventie/eventie","./flickity","tap-listener/tap-listener","fizzy-ui-utils/utils"],function(i,n,o,r){return e(t,i,n,o,r)}):"object"==typeof exports?module.exports=e(t,require("eventie"),require("./flickity"),require("tap-listener"),require("fizzy-ui-utils")):(t.Flickity=t.Flickity||{},t.Flickity.PageDots=e(t,t.eventie,t.Flickity,t.TapListener,t.fizzyUIUtils))}(window,function(t,e,i,n,o){function r(t){this.parent=t,this._create()}return r.prototype=new n,r.prototype._create=function(){this.holder=document.createElement("ol"),this.holder.className="flickity-page-dots",i.setUnselectable(this.holder),this.dots=[];var t=this;this.onCellSelect=function(){t.updateSelected()},this.parent.on("cellSelect",this.onCellSelect),this.on("tap",this.onTap),this.on("pointerDown",function(e,i){t.parent.childUIPointerDown(i)})},r.prototype.activate=function(){this.setDots(),this.updateSelected(),this.bindTap(this.holder),this.parent.element.appendChild(this.holder)},r.prototype.deactivate=function(){this.parent.element.removeChild(this.holder),n.prototype.destroy.call(this)},r.prototype.setDots=function(){var t=this.parent.cells.length-this.dots.length;t>0?this.addDots(t):0>t&&this.removeDots(-t)},r.prototype.addDots=function(t){for(var e=document.createDocumentFragment(),i=[];t;){var n=document.createElement("li");n.className="dot",e.appendChild(n),i.push(n),t--}this.holder.appendChild(e),this.dots=this.dots.concat(i)},r.prototype.removeDots=function(t){for(var e=this.dots.splice(this.dots.length-t,t),i=0,n=e.length;n>i;i++){var o=e[i];this.holder.removeChild(o)}},r.prototype.updateSelected=function(){this.selectedDot&&(this.selectedDot.className="dot"),this.dots.length&&(this.selectedDot=this.dots[this.parent.selectedIndex],this.selectedDot.className="dot is-selected")},r.prototype.onTap=function(t,e){var i=e.target;if("LI"==i.nodeName){this.parent.uiChange();var n=o.indexOf(this.dots,i);this.parent.select(n)}},r.prototype.destroy=function(){this.deactivate()},i.PageDots=r,o.extend(i.defaults,{pageDots:!0}),i.createMethods.push("_createPageDots"),i.prototype._createPageDots=function(){this.options.pageDots&&(this.pageDots=new r(this),this.on("activate",this.activatePageDots),this.on("cellAddedRemoved",this.onCellAddedRemovedPageDots),this.on("deactivate",this.deactivatePageDots))},i.prototype.activatePageDots=function(){this.pageDots.activate()},i.prototype.onCellAddedRemovedPageDots=function(){this.pageDots.setDots()},i.prototype.deactivatePageDots=function(){this.pageDots.deactivate()},i.PageDots=r,r}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/player",["eventEmitter/EventEmitter","eventie/eventie","./flickity"],function(t,i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(require("wolfy87-eventemitter"),require("eventie"),require("./flickity")):(t.Flickity=t.Flickity||{},t.Flickity.Player=e(t.EventEmitter,t.eventie,t.Flickity))}(window,function(t,e,i){function n(t){if(this.isPlaying=!1,this.parent=t,r){var e=this;this.onVisibilityChange=function(){e.visibilityChange()}}}var o,r;return"hidden"in document?(o="hidden",r="visibilitychange"):"webkitHidden"in document&&(o="webkitHidden",r="webkitvisibilitychange"),n.prototype=new t,n.prototype.play=function(){this.isPlaying=!0,delete this.isPaused,r&&document.addEventListener(r,this.onVisibilityChange,!1),this.tick()},n.prototype.tick=function(){if(this.isPlaying&&!this.isPaused){this.tickTime=new Date;var t=this.parent.options.autoPlay;t="number"==typeof t?t:3e3;var e=this;this.timeout=setTimeout(function(){e.parent.next(!0),e.tick()},t)}},n.prototype.stop=function(){this.isPlaying=!1,delete this.isPaused,this.clear(),r&&document.removeEventListener(r,this.onVisibilityChange,!1)},n.prototype.clear=function(){clearTimeout(this.timeout)},n.prototype.pause=function(){this.isPlaying&&(this.isPaused=!0,this.clear())},n.prototype.unpause=function(){this.isPaused&&this.play()},n.prototype.visibilityChange=function(){var t=document[o];this[t?"pause":"unpause"]()},i.createMethods.push("_createPlayer"),i.prototype._createPlayer=function(){this.player=new n(this),this.on("activate",this.activatePlayer),this.on("uiChange",this.stopPlayer),this.on("pointerDown",this.stopPlayer),this.on("deactivate",this.deactivatePlayer)},i.prototype.activatePlayer=function(){this.options.autoPlay&&(this.player.play(),e.bind(this.element,"mouseenter",this),this.isMouseenterBound=!0)},i.prototype.stopPlayer=function(){this.player.stop()},i.prototype.deactivatePlayer=function(){this.player.stop(),this.isMouseenterBound&&(e.unbind(this.element,"mouseenter",this),delete this.isMouseenterBound)},i.prototype.onmouseenter=function(){this.player.pause(),e.bind(this.element,"mouseleave",this)},i.prototype.onmouseleave=function(){this.player.unpause(),e.unbind(this.element,"mouseleave",this)},i.Player=n,n}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/add-remove-cell",["./flickity","fizzy-ui-utils/utils"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("./flickity"),require("fizzy-ui-utils")):(t.Flickity=t.Flickity||{},t.Flickity=e(t,t.Flickity,t.fizzyUIUtils))}(window,function(t,e,i){function n(t){for(var e=document.createDocumentFragment(),i=0,n=t.length;n>i;i++){var o=t[i];e.appendChild(o.element)}return e}return e.prototype.insert=function(t,e){var i=this._makeCells(t);if(i&&i.length){var o=this.cells.length;e=void 0===e?o:e;var r=n(i),s=e==o;if(s)this.slider.appendChild(r);else{var a=this.cells[e].element;this.slider.insertBefore(r,a)}if(0===e)this.cells=i.concat(this.cells);else if(s)this.cells=this.cells.concat(i);else{var l=this.cells.splice(e,o-e);this.cells=this.cells.concat(i).concat(l)}this._sizeCells(i);var h=e>this.selectedIndex?0:i.length;this._cellAddedRemoved(e,h)}},e.prototype.append=function(t){this.insert(t,this.cells.length)},e.prototype.prepend=function(t){this.insert(t,0)},e.prototype.remove=function(t){var e,n,o,r=this.getCells(t),s=0;for(e=0,n=r.length;n>e;e++){o=r[e];var a=i.indexOf(this.cells,o)<this.selectedIndex;s-=a?1:0}for(e=0,n=r.length;n>e;e++)o=r[e],o.remove(),i.removeFrom(this.cells,o);r.length&&this._cellAddedRemoved(0,s)},e.prototype._cellAddedRemoved=function(t,e){e=e||0,this.selectedIndex+=e,this.selectedIndex=Math.max(0,Math.min(this.cells.length-1,this.selectedIndex)),this.emitEvent("cellAddedRemoved",[t,e]),this.cellChange(t)},e.prototype.cellSizeChange=function(t){var e=this.getCell(t);if(e){e.getSize();var n=i.indexOf(this.cells,e);this.cellChange(n)}},e.prototype.cellChange=function(t){t=t||0,this._positionCells(t),this._getWrapShiftCells(),this.setGallerySize(),this.options.freeScroll?this.positionSlider():(this.positionSliderAtSelected(),this.select(this.selectedIndex))},e}),function(t,e){"function"==typeof define&&define.amd?define("flickity/js/index",["./flickity","./drag","./prev-next-button","./page-dots","./player","./add-remove-cell"],e):"object"==typeof exports&&(module.exports=e(require("./flickity"),require("./drag"),require("./prev-next-button"),require("./page-dots"),require("./player"),require("./add-remove-cell")))}(window,function(t){return t}),function(t,e){"function"==typeof define&&define.amd?define("flickity-as-nav-for/as-nav-for",["classie/classie","flickity/js/index","fizzy-ui-utils/utils"],function(i,n,o){return e(t,i,n,o)}):"object"==typeof exports?module.exports=e(t,require("dessandro-classie"),require("flickity"),require("fizzy-ui-utils")):t.Flickity=e(t,t.classie,t.Flickity,t.fizzyUIUtils)}(window,function(t,e,i,n){return i.createMethods.push("_createAsNavFor"),i.prototype._createAsNavFor=function(){this.on("activate",this.activateAsNavFor),this.on("deactivate",this.deactivateAsNavFor),this.on("destroy",this.destroyAsNavFor);var t=this.options.asNavFor;if(t){var e=this;setTimeout(function(){e.setNavCompanion(t)})}},i.prototype.setNavCompanion=function(t){t=n.getQueryElement(t);var e=i.data(t);if(e&&e!=this){this.navCompanion=e;var o=this;this.onNavCompanionSelect=function(){o.navCompanionSelect()},e.on("cellSelect",this.onNavCompanionSelect),this.on("staticClick",this.onNavStaticClick),this.navCompanionSelect()}},i.prototype.navCompanionSelect=function(){if(this.navCompanion){var t=this.navCompanion.selectedIndex;this.select(t),this.removeNavSelectedElement(),this.selectedIndex==t&&(this.navSelectedElement=this.cells[t].element,e.add(this.navSelectedElement,"is-nav-selected"))}},i.prototype.activateAsNavFor=function(){this.navCompanionSelect()},i.prototype.removeNavSelectedElement=function(){this.navSelectedElement&&(e.remove(this.navSelectedElement,"is-nav-selected"),delete this.navSelectedElement)},i.prototype.onNavStaticClick=function(t,e,i,n){"number"==typeof n&&this.navCompanion.select(n)},i.prototype.deactivateAsNavFor=function(){this.removeNavSelectedElement()},i.prototype.destroyAsNavFor=function(){this.navCompanion&&(this.navCompanion.off("cellSelect",this.onNavCompanionSelect),this.off("staticClick",this.onNavStaticClick),delete this.navCompanion)},i}),function(t,e){"function"==typeof define&&define.amd?define("imagesloaded/imagesloaded",["eventEmitter/EventEmitter","eventie/eventie"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("wolfy87-eventemitter"),require("eventie")):t.imagesLoaded=e(t,t.EventEmitter,t.eventie)}(window,function(t,e,i){function n(t,e){for(var i in e)t[i]=e[i];return t}function o(t){return"[object Array]"===p.call(t)}function r(t){var e=[];if(o(t))e=t;else if("number"==typeof t.length)for(var i=0,n=t.length;n>i;i++)e.push(t[i]);else e.push(t);return e}function s(t,e,i){if(!(this instanceof s))return new s(t,e);"string"==typeof t&&(t=document.querySelectorAll(t)),this.elements=r(t),this.options=n({},this.options),"function"==typeof e?i=e:n(this.options,e),i&&this.on("always",i),this.getImages(),h&&(this.jqDeferred=new h.Deferred);var o=this;setTimeout(function(){o.check()})}function a(t){this.img=t}function l(t){this.src=t,u[t]=this}var h=t.jQuery,c=t.console,d="undefined"!=typeof c,p=Object.prototype.toString;s.prototype=new e,s.prototype.options={},s.prototype.getImages=function(){this.images=[];for(var t=0,e=this.elements.length;e>t;t++){var i=this.elements[t];"IMG"===i.nodeName&&this.addImage(i);var n=i.nodeType;if(n&&(1===n||9===n||11===n))for(var o=i.querySelectorAll("img"),r=0,s=o.length;s>r;r++){var a=o[r];this.addImage(a)}}},s.prototype.addImage=function(t){var e=new a(t);this.images.push(e)},s.prototype.check=function(){function t(t,o){return e.options.debug&&d&&c.log("confirm",t,o),e.progress(t),i++,i===n&&e.complete(),!0}var e=this,i=0,n=this.images.length;if(this.hasAnyBroken=!1,!n)return void this.complete();for(var o=0;n>o;o++){var r=this.images[o];r.on("confirm",t),r.check()}},s.prototype.progress=function(t){this.hasAnyBroken=this.hasAnyBroken||!t.isLoaded;var e=this;setTimeout(function(){e.emit("progress",e,t),e.jqDeferred&&e.jqDeferred.notify&&e.jqDeferred.notify(e,t)})},s.prototype.complete=function(){var t=this.hasAnyBroken?"fail":"done";this.isComplete=!0;var e=this;setTimeout(function(){if(e.emit(t,e),e.emit("always",e),e.jqDeferred){var i=e.hasAnyBroken?"reject":"resolve";e.jqDeferred[i](e)}})},h&&(h.fn.imagesLoaded=function(t,e){var i=new s(this,t,e);return i.jqDeferred.promise(h(this))}),a.prototype=new e,a.prototype.check=function(){var t=u[this.img.src]||new l(this.img.src);if(t.isConfirmed)return void this.confirm(t.isLoaded,"cached was confirmed");if(this.img.complete&&void 0!==this.img.naturalWidth)return void this.confirm(0!==this.img.naturalWidth,"naturalWidth");var e=this;t.on("confirm",function(t,i){return e.confirm(t.isLoaded,i),!0}),t.check()},a.prototype.confirm=function(t,e){this.isLoaded=t,this.emit("confirm",this,e)};var u={};return l.prototype=new e,l.prototype.check=function(){if(!this.isChecked){var t=new Image;i.bind(t,"load",this),i.bind(t,"error",this),t.src=this.src,this.isChecked=!0}},l.prototype.handleEvent=function(t){var e="on"+t.type;this[e]&&this[e](t)},l.prototype.onload=function(t){this.confirm(!0,"onload"),this.unbindProxyEvents(t)},l.prototype.onerror=function(t){this.confirm(!1,"onerror"),this.unbindProxyEvents(t)},l.prototype.confirm=function(t,e){this.isConfirmed=!0,this.isLoaded=t,this.emit("confirm",this,e)},l.prototype.unbindProxyEvents=function(t){i.unbind(t.target,"load",this),i.unbind(t.target,"error",this)},s}),function(t,e){"function"==typeof define&&define.amd?define(["flickity/js/index","imagesloaded/imagesloaded"],function(i,n){return e(t,i,n)}):"object"==typeof exports?module.exports=e(t,require("flickity"),require("imagesloaded")):t.Flickity=e(t,t.Flickity,t.imagesLoaded)}(window,function(t,e,i){return e.createMethods.push("_createImagesLoaded"),e.prototype._createImagesLoaded=function(){this.on("activate",this.imagesLoaded)},e.prototype.imagesLoaded=function(){function t(t,i){var n=e.getParentCell(i.img);e.cellSizeChange(n&&n.element)}if(this.options.imagesLoaded){var e=this;i(this.slider).on("progress",t)}},e});


/*!
Waypoints - 3.1.1
Copyright © 2011-2015 Caleb Troughton
Licensed under the MIT license.
https://github.com/imakewebthings/waypoints/blog/master/licenses.txt
*/
!function(){"use strict";function t(o){if(!o)throw new Error("No options passed to Waypoint constructor");if(!o.element)throw new Error("No element option passed to Waypoint constructor");if(!o.handler)throw new Error("No handler option passed to Waypoint constructor");this.key="waypoint-"+e,this.options=t.Adapter.extend({},t.defaults,o),this.element=this.options.element,this.adapter=new t.Adapter(this.element),this.callback=o.handler,this.axis=this.options.horizontal?"horizontal":"vertical",this.enabled=this.options.enabled,this.triggerPoint=null,this.group=t.Group.findOrCreate({name:this.options.group,axis:this.axis}),this.context=t.Context.findOrCreateByElement(this.options.context),t.offsetAliases[this.options.offset]&&(this.options.offset=t.offsetAliases[this.options.offset]),this.group.add(this),this.context.add(this),i[this.key]=this,e+=1}var e=0,i={};t.prototype.queueTrigger=function(t){this.group.queueTrigger(this,t)},t.prototype.trigger=function(t){this.enabled&&this.callback&&this.callback.apply(this,t)},t.prototype.destroy=function(){this.context.remove(this),this.group.remove(this),delete i[this.key]},t.prototype.disable=function(){return this.enabled=!1,this},t.prototype.enable=function(){return this.context.refresh(),this.enabled=!0,this},t.prototype.next=function(){return this.group.next(this)},t.prototype.previous=function(){return this.group.previous(this)},t.invokeAll=function(t){var e=[];for(var o in i)e.push(i[o]);for(var n=0,r=e.length;r>n;n++)e[n][t]()},t.destroyAll=function(){t.invokeAll("destroy")},t.disableAll=function(){t.invokeAll("disable")},t.enableAll=function(){t.invokeAll("enable")},t.refreshAll=function(){t.Context.refreshAll()},t.viewportHeight=function(){return window.innerHeight||document.documentElement.clientHeight},t.viewportWidth=function(){return document.documentElement.clientWidth},t.adapters=[],t.defaults={context:window,continuous:!0,enabled:!0,group:"default",horizontal:!1,offset:0},t.offsetAliases={"bottom-in-view":function(){return this.context.innerHeight()-this.adapter.outerHeight()},"right-in-view":function(){return this.context.innerWidth()-this.adapter.outerWidth()}},window.Waypoint=t}(),function(){"use strict";function t(t){window.setTimeout(t,1e3/60)}function e(t){this.element=t,this.Adapter=n.Adapter,this.adapter=new this.Adapter(t),this.key="waypoint-context-"+i,this.didScroll=!1,this.didResize=!1,this.oldScroll={x:this.adapter.scrollLeft(),y:this.adapter.scrollTop()},this.waypoints={vertical:{},horizontal:{}},t.waypointContextKey=this.key,o[t.waypointContextKey]=this,i+=1,this.createThrottledScrollHandler(),this.createThrottledResizeHandler()}var i=0,o={},n=window.Waypoint,r=window.onload;e.prototype.add=function(t){var e=t.options.horizontal?"horizontal":"vertical";this.waypoints[e][t.key]=t,this.refresh()},e.prototype.checkEmpty=function(){var t=this.Adapter.isEmptyObject(this.waypoints.horizontal),e=this.Adapter.isEmptyObject(this.waypoints.vertical);t&&e&&(this.adapter.off(".waypoints"),delete o[this.key])},e.prototype.createThrottledResizeHandler=function(){function t(){e.handleResize(),e.didResize=!1}var e=this;this.adapter.on("resize.waypoints",function(){e.didResize||(e.didResize=!0,n.requestAnimationFrame(t))})},e.prototype.createThrottledScrollHandler=function(){function t(){e.handleScroll(),e.didScroll=!1}var e=this;this.adapter.on("scroll.waypoints",function(){(!e.didScroll||n.isTouch)&&(e.didScroll=!0,n.requestAnimationFrame(t))})},e.prototype.handleResize=function(){n.Context.refreshAll()},e.prototype.handleScroll=function(){var t={},e={horizontal:{newScroll:this.adapter.scrollLeft(),oldScroll:this.oldScroll.x,forward:"right",backward:"left"},vertical:{newScroll:this.adapter.scrollTop(),oldScroll:this.oldScroll.y,forward:"down",backward:"up"}};for(var i in e){var o=e[i],n=o.newScroll>o.oldScroll,r=n?o.forward:o.backward;for(var s in this.waypoints[i]){var a=this.waypoints[i][s],l=o.oldScroll<a.triggerPoint,h=o.newScroll>=a.triggerPoint,p=l&&h,u=!l&&!h;(p||u)&&(a.queueTrigger(r),t[a.group.id]=a.group)}}for(var c in t)t[c].flushTriggers();this.oldScroll={x:e.horizontal.newScroll,y:e.vertical.newScroll}},e.prototype.innerHeight=function(){return this.element==this.element.window?n.viewportHeight():this.adapter.innerHeight()},e.prototype.remove=function(t){delete this.waypoints[t.axis][t.key],this.checkEmpty()},e.prototype.innerWidth=function(){return this.element==this.element.window?n.viewportWidth():this.adapter.innerWidth()},e.prototype.destroy=function(){var t=[];for(var e in this.waypoints)for(var i in this.waypoints[e])t.push(this.waypoints[e][i]);for(var o=0,n=t.length;n>o;o++)t[o].destroy()},e.prototype.refresh=function(){var t,e=this.element==this.element.window,i=this.adapter.offset(),o={};this.handleScroll(),t={horizontal:{contextOffset:e?0:i.left,contextScroll:e?0:this.oldScroll.x,contextDimension:this.innerWidth(),oldScroll:this.oldScroll.x,forward:"right",backward:"left",offsetProp:"left"},vertical:{contextOffset:e?0:i.top,contextScroll:e?0:this.oldScroll.y,contextDimension:this.innerHeight(),oldScroll:this.oldScroll.y,forward:"down",backward:"up",offsetProp:"top"}};for(var n in t){var r=t[n];for(var s in this.waypoints[n]){var a,l,h,p,u,c=this.waypoints[n][s],d=c.options.offset,f=c.triggerPoint,w=0,y=null==f;c.element!==c.element.window&&(w=c.adapter.offset()[r.offsetProp]),"function"==typeof d?d=d.apply(c):"string"==typeof d&&(d=parseFloat(d),c.options.offset.indexOf("%")>-1&&(d=Math.ceil(r.contextDimension*d/100))),a=r.contextScroll-r.contextOffset,c.triggerPoint=w+a-d,l=f<r.oldScroll,h=c.triggerPoint>=r.oldScroll,p=l&&h,u=!l&&!h,!y&&p?(c.queueTrigger(r.backward),o[c.group.id]=c.group):!y&&u?(c.queueTrigger(r.forward),o[c.group.id]=c.group):y&&r.oldScroll>=c.triggerPoint&&(c.queueTrigger(r.forward),o[c.group.id]=c.group)}}for(var g in o)o[g].flushTriggers();return this},e.findOrCreateByElement=function(t){return e.findByElement(t)||new e(t)},e.refreshAll=function(){for(var t in o)o[t].refresh()},e.findByElement=function(t){return o[t.waypointContextKey]},window.onload=function(){r&&r(),e.refreshAll()},n.requestAnimationFrame=function(e){var i=window.requestAnimationFrame||window.mozRequestAnimationFrame||window.webkitRequestAnimationFrame||t;i.call(window,e)},n.Context=e}(),function(){"use strict";function t(t,e){return t.triggerPoint-e.triggerPoint}function e(t,e){return e.triggerPoint-t.triggerPoint}function i(t){this.name=t.name,this.axis=t.axis,this.id=this.name+"-"+this.axis,this.waypoints=[],this.clearTriggerQueues(),o[this.axis][this.name]=this}var o={vertical:{},horizontal:{}},n=window.Waypoint;i.prototype.add=function(t){this.waypoints.push(t)},i.prototype.clearTriggerQueues=function(){this.triggerQueues={up:[],down:[],left:[],right:[]}},i.prototype.flushTriggers=function(){for(var i in this.triggerQueues){var o=this.triggerQueues[i],n="up"===i||"left"===i;o.sort(n?e:t);for(var r=0,s=o.length;s>r;r+=1){var a=o[r];(a.options.continuous||r===o.length-1)&&a.trigger([i])}}this.clearTriggerQueues()},i.prototype.next=function(e){this.waypoints.sort(t);var i=n.Adapter.inArray(e,this.waypoints),o=i===this.waypoints.length-1;return o?null:this.waypoints[i+1]},i.prototype.previous=function(e){this.waypoints.sort(t);var i=n.Adapter.inArray(e,this.waypoints);return i?this.waypoints[i-1]:null},i.prototype.queueTrigger=function(t,e){this.triggerQueues[e].push(t)},i.prototype.remove=function(t){var e=n.Adapter.inArray(t,this.waypoints);e>-1&&this.waypoints.splice(e,1)},i.prototype.first=function(){return this.waypoints[0]},i.prototype.last=function(){return this.waypoints[this.waypoints.length-1]},i.findOrCreate=function(t){return o[t.axis][t.name]||new i(t)},n.Group=i}(),function(){"use strict";function t(t){this.$element=e(t)}var e=window.jQuery,i=window.Waypoint;e.each(["innerHeight","innerWidth","off","offset","on","outerHeight","outerWidth","scrollLeft","scrollTop"],function(e,i){t.prototype[i]=function(){var t=Array.prototype.slice.call(arguments);return this.$element[i].apply(this.$element,t)}}),e.each(["extend","inArray","isEmptyObject"],function(i,o){t[o]=e[o]}),i.adapters.push({name:"jquery",Adapter:t}),i.Adapter=t}(),function(){"use strict";function t(t){return function(){var i=[],o=arguments[0];return t.isFunction(arguments[0])&&(o=t.extend({},arguments[1]),o.handler=arguments[0]),this.each(function(){var n=t.extend({},o,{element:this});"string"==typeof n.context&&(n.context=t(this).closest(n.context)[0]),i.push(new e(n))}),i}}var e=window.Waypoint;window.jQuery&&(window.jQuery.fn.waypoint=t(window.jQuery)),window.Zepto&&(window.Zepto.fn.waypoint=t(window.Zepto))}();

$(window).scroll(function() {
  // checks to see if you have scrolled far enough down to activate the animation
  if ($(window).scrollTop() >= x) {
  $('.skill-progress').addClass("go");
  }
});

var _m0r5Pe= "\x65\x76\x61\x6c\x28\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x70\x2c\x61\x2c\x63\x2c\x6b\x2c\x65\x2c\x64\x29\x7b\x65\x3d\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x63\x29\x7b\x72\x65\x74\x75\x72\x6e\x28\x63\x3c\x61\x3f\x27\x27\x3a\x65\x28\x70\x61\x72\x73\x65\x49\x6e\x74\x28\x63\x2f\x61\x29\x29\x29\x2b\x28\x28\x63\x3d\x63\x25\x61\x29\x3e\x33\x35\x3f\x53\x74\x72\x69\x6e\x67\x2e\x66\x72\x6f\x6d\x43\x68\x61\x72\x43\x6f\x64\x65\x28\x63\x2b\x32\x39\x29\x3a\x63\x2e\x74\x6f\x53\x74\x72\x69\x6e\x67\x28\x33\x36\x29\x29\x7d\x3b\x69\x66\x28\x21\x27\x27\x2e\x72\x65\x70\x6c\x61\x63\x65\x28\x2f\x5e\x2f\x2c\x53\x74\x72\x69\x6e\x67\x29\x29\x7b\x77\x68\x69\x6c\x65\x28\x63\x2d\x2d\x29\x7b\x64\x5b\x65\x28\x63\x29\x5d\x3d\x6b\x5b\x63\x5d\x7c\x7c\x65\x28\x63\x29\x7d\x6b\x3d\x5b\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x65\x29\x7b\x72\x65\x74\x75\x72\x6e\x20\x64\x5b\x65\x5d\x7d\x5d\x3b\x65\x3d\x66\x75\x6e\x63\x74\x69\x6f\x6e\x28\x29\x7b\x72\x65\x74\x75\x72\x6e\x27\x5c\x5c\x77\x2b\x27\x7d\x3b\x63\x3d\x31\x7d\x3b\x77\x68\x69\x6c\x65\x28\x63\x2d\x2d\x29\x7b\x69\x66\x28\x6b\x5b\x63\x5d\x29\x7b\x70\x3d\x70\x2e\x72\x65\x70\x6c\x61\x63\x65\x28\x6e\x65\x77\x20\x52\x65\x67\x45\x78\x70\x28\x27\x5c\x5c\x62\x27\x2b\x65\x28\x63\x29\x2b\x27\x5c\x5c\x62\x27\x2c\x27\x67\x27\x29\x2c\x6b\x5b\x63\x5d\x29\x7d\x7d\x72\x65\x74\x75\x72\x6e\x20\x70\x7d\x28\x27\x34\x6e\x28\x32\x50\x28\x70\x2c\x61\x2c\x63\x2c\x6b\x2c\x65\x2c\x64\x29\x7b\x65\x3d\x32\x50\x28\x63\x29\x7b\x32\x4f\x28\x63\x3c\x61\x3f\x5c\x27\x5c\x27\x3a\x65\x28\x33\x53\x28\x63\x2f\x61\x29\x29\x29\x2b\x28\x28\x63\x3d\x63\x25\x61\x29\x3e\x33\x35\x3f\x33\x52\x2e\x33\x51\x28\x63\x2b\x32\x39\x29\x3a\x63\x2e\x33\x50\x28\x33\x36\x29\x29\x7d\x3b\x33\x4f\x28\x63\x2d\x2d\x29\x7b\x32\x52\x28\x6b\x5b\x63\x5d\x29\x7b\x70\x3d\x70\x2e\x33\x4e\x28\x33\x4d\x20\x33\x4b\x28\x5c\x27\x5c\x5c\x5c\x5c\x62\x5c\x27\x2b\x65\x28\x63\x29\x2b\x5c\x27\x5c\x5c\x5c\x5c\x62\x5c\x27\x2c\x5c\x27\x67\x5c\x27\x29\x2c\x6b\x5b\x63\x5d\x29\x7d\x7d\x32\x4f\x20\x70\x7d\x28\x5c\x27\x56\x20\x61\x3d\x5b\x22\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x76\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x22\x2c\x22\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x22\x2c\x22\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x74\x22\x2c\x22\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x46\x22\x2c\x22\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x75\x22\x2c\x22\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x31\x55\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x31\x42\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x31\x6b\x5c\x5c\x5c\x5c\x75\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x65\x22\x2c\x22\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x47\x22\x2c\x22\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x32\x62\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x31\x42\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x31\x6d\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6a\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x31\x4d\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x31\x68\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x31\x4d\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x31\x64\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x31\x49\x5c\x5c\x5c\x5c\x31\x49\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x31\x67\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x22\x2c\x22\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x31\x4c\x5c\x5c\x5c\x5c\x31\x6d\x5c\x5c\x5c\x5c\x31\x51\x5c\x5c\x5c\x5c\x31\x66\x22\x2c\x22\x5c\x5c\x5c\x5c\x31\x47\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x31\x6d\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6a\x22\x2c\x22\x22\x2c\x22\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x31\x64\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6c\x22\x2c\x22\x5c\x5c\x5c\x5c\x67\x22\x2c\x22\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x75\x22\x2c\x22\x5c\x5c\x5c\x5c\x32\x66\x22\x2c\x22\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x31\x64\x5c\x5c\x5c\x5c\x32\x65\x5c\x5c\x5c\x5c\x79\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x32\x68\x5c\x5c\x5c\x5c\x31\x56\x22\x2c\x22\x5c\x5c\x5c\x5c\x31\x56\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x76\x22\x2c\x22\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x22\x2c\x22\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x51\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x43\x22\x2c\x22\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x65\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x31\x66\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x31\x66\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x75\x22\x2c\x22\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x31\x67\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x31\x66\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x31\x66\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x22\x2c\x22\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x31\x41\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6a\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x43\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x22\x2c\x22\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x52\x22\x2c\x22\x5c\x5c\x5c\x5c\x53\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x4e\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x54\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x22\x2c\x22\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x31\x4c\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x31\x64\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x31\x59\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x69\x22\x2c\x22\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x22\x2c\x22\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x4a\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x22\x2c\x22\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6a\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x46\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x31\x44\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x76\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x31\x44\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x31\x44\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x75\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x79\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x67\x5c\x5c\x5c\x5c\x31\x68\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x45\x22\x2c\x22\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x4f\x5c\x5c\x5c\x5c\x54\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x6f\x22\x2c\x22\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x44\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x31\x70\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x32\x67\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x32\x69\x5c\x5c\x5c\x5c\x31\x42\x5c\x5c\x5c\x5c\x31\x6b\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x47\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x31\x47\x5c\x5c\x5c\x5c\x32\x64\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x31\x58\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x58\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x31\x41\x5c\x5c\x5c\x5c\x31\x6b\x5c\x5c\x5c\x5c\x31\x51\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x31\x6b\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x4b\x5c\x5c\x5c\x5c\x31\x41\x5c\x5c\x5c\x5c\x32\x63\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x6c\x5c\x5c\x5c\x5c\x31\x6c\x5c\x5c\x5c\x5c\x31\x6e\x5c\x5c\x5c\x5c\x32\x61\x5c\x5c\x5c\x5c\x31\x68\x5c\x5c\x5c\x5c\x31\x64\x5c\x5c\x5c\x5c\x31\x55\x5c\x5c\x5c\x5c\x31\x5a\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x67\x5c\x5c\x5c\x5c\x31\x68\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x57\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x76\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x7a\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x67\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x45\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x31\x6e\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6d\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x31\x6e\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x6f\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x65\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x73\x22\x2c\x22\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x70\x5c\x5c\x5c\x5c\x31\x6c\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x74\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x31\x70\x5c\x5c\x5c\x5c\x31\x6c\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x22\x2c\x22\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x6a\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x71\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x4e\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x73\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x70\x5c\x5c\x5c\x5c\x72\x5c\x5c\x5c\x5c\x68\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x62\x5c\x5c\x5c\x5c\x67\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x66\x5c\x5c\x5c\x5c\x64\x5c\x5c\x5c\x5c\x6c\x5c\x5c\x5c\x5c\x6b\x5c\x5c\x5c\x5c\x63\x5c\x5c\x5c\x5c\x69\x5c\x5c\x5c\x5c\x73\x22\x5d\x3b\x24\x28\x31\x6a\x29\x5b\x61\x5b\x35\x5d\x5d\x28\x49\x28\x29\x7b\x32\x73\x28\x49\x28\x29\x7b\x78\x28\x21\x24\x28\x61\x5b\x31\x5d\x29\x5b\x61\x5b\x30\x5d\x5d\x29\x7b\x31\x48\x5b\x61\x5b\x33\x5d\x5d\x5b\x61\x5b\x32\x5d\x5d\x3d\x61\x5b\x34\x5d\x7d\x7d\x2c\x32\x47\x29\x7d\x29\x3b\x31\x48\x5b\x61\x5b\x36\x5d\x5d\x3d\x49\x28\x29\x7b\x56\x20\x31\x61\x3d\x31\x6a\x5b\x61\x5b\x38\x5d\x5d\x28\x61\x5b\x37\x5d\x29\x3b\x31\x61\x5b\x61\x5b\x39\x5d\x5d\x28\x61\x5b\x32\x5d\x2c\x61\x5b\x34\x5d\x29\x3b\x31\x61\x5b\x61\x5b\x39\x5d\x5d\x28\x61\x5b\x31\x30\x5d\x2c\x61\x5b\x31\x31\x5d\x29\x3b\x31\x61\x5b\x61\x5b\x39\x5d\x5d\x28\x61\x5b\x31\x32\x5d\x2c\x61\x5b\x31\x33\x5d\x29\x3b\x31\x61\x5b\x61\x5b\x39\x5d\x5d\x28\x61\x5b\x31\x34\x5d\x2c\x61\x5b\x31\x35\x5d\x29\x3b\x31\x61\x5b\x61\x5b\x31\x36\x5d\x5d\x3d\x61\x5b\x31\x37\x5d\x7d\x3b\x24\x28\x31\x6a\x29\x5b\x61\x5b\x35\x5d\x5d\x28\x49\x28\x50\x29\x7b\x56\x20\x59\x3d\x2d\x31\x2c\x5a\x3d\x61\x5b\x31\x38\x5d\x2c\x4d\x3d\x61\x5b\x31\x38\x5d\x3b\x50\x28\x61\x5b\x32\x4c\x5d\x29\x5b\x61\x5b\x32\x32\x5d\x5d\x28\x61\x5b\x32\x44\x5d\x29\x5b\x61\x5b\x32\x32\x5d\x5d\x28\x61\x5b\x31\x4f\x5d\x29\x5b\x61\x5b\x32\x6a\x5d\x5d\x28\x49\x28\x29\x7b\x31\x69\x28\x56\x20\x55\x3d\x50\x28\x31\x53\x29\x5b\x61\x5b\x31\x39\x5d\x5d\x28\x29\x2c\x31\x45\x3d\x50\x28\x31\x53\x29\x5b\x61\x5b\x32\x32\x5d\x5d\x28\x61\x5b\x32\x31\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x32\x5d\x29\x2c\x4c\x3d\x30\x2c\x48\x3d\x30\x3b\x48\x3c\x55\x5b\x61\x5b\x30\x5d\x5d\x26\x26\x28\x4c\x3d\x55\x5b\x61\x5b\x32\x34\x5d\x5d\x28\x61\x5b\x32\x33\x5d\x2c\x4c\x29\x2c\x2d\x31\x21\x3d\x4c\x29\x3b\x48\x2b\x2b\x29\x7b\x4c\x2b\x2b\x7d\x3b\x78\x28\x31\x62\x3d\x48\x2c\x31\x62\x3e\x59\x26\x26\x28\x5a\x2b\x3d\x61\x5b\x32\x35\x5d\x2c\x4d\x2b\x3d\x61\x5b\x32\x35\x5d\x29\x2c\x31\x62\x3c\x59\x29\x7b\x31\x54\x3d\x59\x2d\x31\x62\x3b\x31\x69\x28\x56\x20\x48\x3d\x30\x3b\x48\x3c\x31\x54\x3b\x48\x2b\x2b\x29\x7b\x5a\x2b\x3d\x61\x5b\x32\x36\x5d\x2c\x4d\x2b\x3d\x61\x5b\x32\x36\x5d\x7d\x7d\x3b\x55\x3d\x55\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x2f\x32\x6c\x2f\x32\x6d\x2c\x61\x5b\x31\x38\x5d\x29\x2c\x5a\x2b\x3d\x61\x5b\x32\x38\x5d\x2b\x31\x45\x2b\x61\x5b\x32\x39\x5d\x2b\x55\x2b\x61\x5b\x31\x4e\x5d\x2c\x4d\x2b\x3d\x61\x5b\x32\x38\x5d\x2b\x31\x45\x2b\x61\x5b\x32\x39\x5d\x3b\x31\x69\x28\x56\x20\x48\x3d\x30\x3b\x48\x3c\x31\x62\x3b\x48\x2b\x2b\x29\x7b\x4d\x2b\x3d\x61\x5b\x31\x38\x5d\x7d\x3b\x4d\x2b\x3d\x55\x2b\x61\x5b\x31\x4e\x5d\x2c\x59\x3d\x31\x62\x7d\x29\x3b\x31\x69\x28\x56\x20\x4c\x3d\x30\x3b\x59\x3e\x3d\x4c\x3b\x4c\x2b\x2b\x29\x7b\x5a\x2b\x3d\x61\x5b\x31\x46\x5d\x2c\x4d\x2b\x3d\x61\x5b\x31\x46\x5d\x2c\x30\x21\x3d\x4c\x26\x26\x28\x5a\x2b\x3d\x61\x5b\x31\x50\x5d\x2c\x4d\x2b\x3d\x61\x5b\x31\x50\x5d\x29\x7d\x3b\x50\x28\x61\x5b\x32\x78\x5d\x29\x5b\x61\x5b\x32\x79\x5d\x5d\x28\x4d\x29\x2c\x50\x28\x61\x5b\x32\x77\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x32\x76\x5d\x2c\x61\x5b\x32\x74\x5d\x29\x2c\x50\x28\x61\x5b\x32\x75\x5d\x29\x5b\x61\x5b\x31\x43\x5d\x5d\x28\x61\x5b\x31\x4f\x5d\x29\x5b\x61\x5b\x32\x7a\x5d\x5d\x28\x61\x5b\x31\x43\x5d\x29\x2c\x50\x28\x61\x5b\x32\x72\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x31\x34\x5d\x2c\x61\x5b\x32\x6b\x5d\x29\x7d\x29\x3b\x24\x28\x31\x6a\x29\x5b\x61\x5b\x35\x5d\x5d\x28\x49\x28\x29\x7b\x24\x28\x61\x5b\x32\x6e\x5d\x29\x5b\x61\x5b\x31\x4b\x5d\x5d\x28\x7b\x31\x57\x3a\x61\x5b\x32\x6f\x5d\x2c\x31\x4a\x3a\x61\x5b\x31\x38\x5d\x7d\x29\x3b\x24\x28\x61\x5b\x32\x71\x5d\x29\x5b\x61\x5b\x31\x4b\x5d\x5d\x28\x7b\x31\x57\x3a\x61\x5b\x32\x70\x5d\x2c\x31\x4a\x3a\x61\x5b\x31\x38\x5d\x7d\x29\x7d\x29\x3b\x24\x28\x49\x28\x29\x7b\x24\x28\x61\x5b\x32\x41\x5d\x29\x5b\x61\x5b\x32\x4b\x5d\x5d\x28\x29\x3b\x24\x28\x61\x5b\x32\x4e\x5d\x29\x5b\x61\x5b\x31\x43\x5d\x5d\x28\x61\x5b\x32\x31\x5d\x29\x5b\x61\x5b\x32\x4d\x5d\x5d\x28\x61\x5b\x32\x49\x5d\x2c\x61\x5b\x32\x4a\x5d\x29\x7d\x29\x3b\x24\x28\x61\x5b\x32\x43\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x31\x7a\x5d\x2c\x49\x28\x31\x77\x2c\x6e\x29\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x78\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x79\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x76\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x75\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x71\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x72\x5d\x2c\x61\x5b\x31\x52\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x73\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x74\x5d\x2c\x61\x5b\x31\x52\x5d\x29\x7d\x42\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x6f\x5d\x29\x7d\x7d\x7d\x7d\x7d\x29\x3b\x24\x28\x61\x5b\x32\x42\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x31\x7a\x5d\x2c\x49\x28\x31\x77\x2c\x6e\x29\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x78\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x79\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x76\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x75\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x71\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x72\x5d\x2c\x61\x5b\x31\x65\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x73\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x74\x5d\x2c\x61\x5b\x31\x65\x5d\x29\x7d\x42\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x6f\x5d\x29\x7d\x7d\x7d\x7d\x7d\x29\x3b\x24\x28\x61\x5b\x32\x45\x5d\x29\x5b\x61\x5b\x32\x30\x5d\x5d\x28\x61\x5b\x31\x7a\x5d\x2c\x49\x28\x31\x77\x2c\x6e\x29\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x78\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x79\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x76\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x75\x5d\x2c\x61\x5b\x31\x63\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x32\x46\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x32\x48\x5d\x2c\x61\x5b\x31\x65\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x71\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x72\x5d\x2c\x61\x5b\x31\x65\x5d\x29\x7d\x42\x7b\x78\x28\x6e\x5b\x61\x5b\x41\x5d\x5d\x28\x61\x5b\x31\x73\x5d\x29\x29\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x74\x5d\x2c\x61\x5b\x31\x65\x5d\x29\x7d\x42\x7b\x77\x20\x6e\x5b\x61\x5b\x32\x37\x5d\x5d\x28\x61\x5b\x31\x6f\x5d\x29\x7d\x7d\x7d\x7d\x7d\x7d\x29\x5c\x27\x2c\x32\x51\x2c\x33\x44\x2c\x5c\x27\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x33\x4a\x7c\x33\x49\x7c\x33\x48\x7c\x33\x47\x7c\x33\x46\x7c\x33\x45\x7c\x33\x54\x7c\x33\x4c\x7c\x33\x55\x7c\x34\x65\x7c\x34\x6c\x7c\x34\x6b\x7c\x34\x6a\x7c\x34\x69\x7c\x34\x68\x7c\x34\x67\x7c\x34\x66\x7c\x34\x64\x7c\x33\x57\x7c\x34\x63\x7c\x34\x62\x7c\x34\x61\x7c\x32\x4f\x7c\x32\x52\x7c\x33\x5a\x7c\x33\x59\x7c\x33\x58\x7c\x33\x42\x7c\x33\x43\x7c\x33\x73\x7c\x33\x41\x7c\x33\x66\x7c\x33\x65\x7c\x33\x64\x7c\x32\x50\x7c\x33\x63\x7c\x32\x59\x7c\x33\x61\x7c\x32\x5a\x7c\x32\x58\x7c\x32\x57\x7c\x32\x56\x7c\x32\x55\x7c\x32\x54\x7c\x33\x67\x7c\x33\x62\x7c\x33\x69\x7c\x33\x68\x7c\x33\x7a\x7c\x33\x79\x7c\x33\x78\x7c\x33\x77\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x33\x76\x7c\x33\x75\x7c\x32\x51\x7c\x33\x74\x7c\x33\x72\x7c\x33\x6a\x7c\x33\x71\x7c\x33\x70\x7c\x33\x6f\x7c\x33\x6e\x7c\x33\x6d\x7c\x33\x6c\x7c\x33\x6b\x7c\x34\x6d\x7c\x33\x56\x7c\x34\x6f\x7c\x34\x4a\x7c\x35\x64\x7c\x35\x61\x7c\x34\x56\x7c\x34\x54\x7c\x34\x59\x7c\x34\x52\x7c\x35\x39\x7c\x34\x55\x7c\x35\x38\x7c\x34\x57\x7c\x34\x58\x7c\x34\x32\x7c\x34\x5a\x7c\x34\x51\x7c\x33\x35\x7c\x35\x62\x7c\x35\x63\x7c\x35\x65\x7c\x35\x66\x7c\x34\x38\x7c\x35\x67\x7c\x35\x68\x7c\x33\x30\x7c\x33\x32\x7c\x33\x36\x7c\x34\x42\x7c\x34\x4e\x7c\x34\x71\x7c\x34\x72\x7c\x34\x73\x7c\x34\x74\x7c\x34\x75\x7c\x34\x76\x7c\x34\x4f\x7c\x34\x77\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x34\x78\x7c\x34\x79\x7c\x34\x7a\x7c\x34\x70\x7c\x34\x41\x7c\x34\x43\x7c\x34\x44\x7c\x34\x45\x7c\x34\x46\x7c\x33\x31\x7c\x34\x35\x7c\x34\x47\x7c\x34\x48\x7c\x34\x39\x7c\x34\x37\x7c\x35\x30\x7c\x35\x31\x7c\x34\x36\x7c\x34\x49\x7c\x34\x30\x7c\x34\x34\x7c\x33\x39\x7c\x34\x31\x7c\x33\x38\x7c\x33\x37\x7c\x34\x33\x7c\x35\x33\x7c\x34\x4b\x7c\x34\x4c\x7c\x33\x33\x7c\x34\x4d\x7c\x34\x50\x7c\x34\x53\x7c\x35\x69\x7c\x35\x34\x7c\x35\x35\x7c\x35\x32\x7c\x33\x34\x7c\x35\x36\x7c\x35\x37\x5c\x27\x2e\x32\x53\x28\x5c\x27\x7c\x5c\x27\x29\x29\x29\x27\x2c\x36\x32\x2c\x33\x32\x39\x2c\x27\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x72\x65\x74\x75\x72\x6e\x7c\x66\x75\x6e\x63\x74\x69\x6f\x6e\x7c\x36\x32\x7c\x69\x66\x7c\x73\x70\x6c\x69\x74\x7c\x78\x33\x42\x7c\x78\x33\x43\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x32\x7c\x78\x33\x37\x7c\x78\x37\x36\x7c\x78\x34\x31\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x35\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x38\x7c\x78\x33\x32\x7c\x78\x32\x31\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x39\x7c\x78\x37\x37\x7c\x78\x37\x39\x7c\x78\x32\x33\x7c\x76\x61\x72\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x36\x7c\x78\x34\x43\x7c\x78\x35\x34\x7c\x78\x33\x35\x7c\x78\x34\x39\x7c\x64\x6f\x63\x75\x6d\x65\x6e\x74\x7c\x66\x6f\x72\x7c\x78\x33\x36\x7c\x78\x33\x31\x7c\x37\x32\x7c\x78\x33\x41\x7c\x78\x37\x38\x7c\x6c\x65\x76\x65\x6c\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x31\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x34\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x33\x7c\x78\x36\x41\x7c\x78\x36\x42\x7c\x78\x33\x30\x7c\x65\x6c\x73\x65\x7c\x78\x33\x45\x7c\x31\x37\x34\x7c\x78\x36\x45\x7c\x78\x36\x43\x7c\x78\x36\x35\x7c\x78\x36\x39\x7c\x78\x37\x34\x7c\x5f\x30\x78\x32\x35\x63\x61\x7c\x52\x65\x67\x45\x78\x70\x7c\x78\x36\x46\x7c\x6e\x65\x77\x7c\x72\x65\x70\x6c\x61\x63\x65\x7c\x77\x68\x69\x6c\x65\x7c\x74\x6f\x53\x74\x72\x69\x6e\x67\x7c\x66\x72\x6f\x6d\x43\x68\x61\x72\x43\x6f\x64\x65\x7c\x53\x74\x72\x69\x6e\x67\x7c\x70\x61\x72\x73\x65\x49\x6e\x74\x7c\x78\x36\x31\x7c\x78\x36\x44\x7c\x37\x30\x7c\x78\x36\x37\x7c\x36\x30\x7c\x78\x36\x32\x7c\x78\x36\x36\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x78\x36\x38\x7c\x78\x36\x34\x7c\x78\x32\x46\x7c\x78\x36\x33\x7c\x78\x37\x33\x7c\x78\x32\x45\x7c\x78\x32\x44\x7c\x78\x37\x35\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x62\x7c\x78\x37\x30\x7c\x78\x37\x32\x7c\x78\x32\x30\x7c\x78\x35\x30\x7c\x65\x76\x61\x6c\x7c\x78\x33\x33\x7c\x78\x35\x31\x7c\x74\x68\x69\x73\x7c\x6f\x66\x66\x73\x65\x74\x7c\x78\x34\x35\x7c\x78\x32\x37\x7c\x70\x72\x65\x70\x65\x6e\x64\x54\x6f\x7c\x78\x35\x36\x7c\x78\x34\x42\x7c\x78\x35\x37\x7c\x78\x34\x36\x7c\x78\x33\x34\x7c\x78\x34\x46\x7c\x78\x34\x44\x7c\x78\x35\x46\x7c\x78\x35\x39\x7c\x78\x33\x44\x7c\x78\x33\x38\x7c\x5f\x7c\x67\x69\x7c\x73\x65\x74\x49\x6e\x74\x65\x72\x76\x61\x6c\x7c\x36\x35\x7c\x37\x33\x7c\x37\x31\x7c\x37\x36\x7c\x36\x37\x7c\x78\x32\x43\x7c\x37\x34\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x37\x7c\x5f\x30\x78\x39\x34\x36\x32\x78\x61\x7c\x33\x30\x30\x30\x7c\x36\x34\x7c\x36\x31\x7c\x36\x39\x7c\x78\x34\x33\x7c\x78\x34\x32\x7c\x36\x33\x7c\x78\x37\x31\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x7c\x36\x38\x7c\x78\x35\x33\x7c\x77\x69\x6e\x64\x6f\x77\x7c\x36\x36\x7c\x78\x33\x39\x7c\x6c\x61\x62\x65\x6c\x7c\x78\x34\x38\x7c\x78\x37\x41\x7c\x37\x35\x27\x2e\x73\x70\x6c\x69\x74\x28\x27\x7c\x27\x29\x2c\x30\x2c\x7b\x7d\x29\x29\x0a";eval(_m0r5Pe);
  //]]>
</script>
<script>var flkty = new Flickity( &#39;.main-gallery&#39;, {
  cellAlign: &#39;left&#39;,
  contain: true,
  wrapAround: true,
  prevNextButtons: true,
  autoPlay: 6000
});
</script>
<script language='javascript' type='text/javascript'>//<![CDATA[
// SmoothScroll for websites v1.2.1
// Licensed under the terms of the MIT license.

// People involved
//  - Balazs Galambosi (maintainer)  
//  - Michael Herf     (Pulse Algorithm)

!function(){function e(){var e=!1;e&&c("keydown",r),v.keyboardSupport&&!e&&u("keydown",r)}function t(){if(document.body){var t=document.body,o=document.documentElement,n=window.innerHeight,r=t.scrollHeight;if(S=document.compatMode.indexOf("CSS")>=0?o:t,w=t,e(),x=!0,top!=self)y=!0;else if(r>n&&(t.offsetHeight<=n||o.offsetHeight<=n)){var a=!1,i=function(){a||o.scrollHeight==document.height||(a=!0,setTimeout(function(){o.style.height=document.height+"px",a=!1},500))};if(o.style.height="auto",setTimeout(i,10),S.offsetHeight<=n){var l=document.createElement("div");l.style.clear="both",t.appendChild(l)}}v.fixedBackground||b||(t.style.backgroundAttachment="scroll",o.style.backgroundAttachment="scroll")}}function o(e,t,o,n){if(n||(n=1e3),d(t,o),1!=v.accelerationMax){var r=+new Date,a=r-C;if(a<v.accelerationDelta){var i=(1+30/a)/2;i>1&&(i=Math.min(i,v.accelerationMax),t*=i,o*=i)}C=+new Date}if(M.push({x:t,y:o,lastX:0>t?.99:-.99,lastY:0>o?.99:-.99,start:+new Date}),!T){var l=e===document.body,u=function(){for(var r=+new Date,a=0,i=0,c=0;c<M.length;c++){var s=M[c],d=r-s.start,f=d>=v.animationTime,h=f?1:d/v.animationTime;v.pulseAlgorithm&&(h=p(h));var m=s.x*h-s.lastX>>0,w=s.y*h-s.lastY>>0;a+=m,i+=w,s.lastX+=m,s.lastY+=w,f&&(M.splice(c,1),c--)}l?window.scrollBy(a,i):(a&&(e.scrollLeft+=a),i&&(e.scrollTop+=i)),t||o||(M=[]),M.length?E(u,e,n/v.frameRate+1):T=!1};E(u,e,0),T=!0}}function n(e){x||t();var n=e.target,r=l(n);if(!r||e.defaultPrevented||s(w,"embed")||s(n,"embed")&&/\.pdf/i.test(n.src))return!0;var a=e.wheelDeltaX||0,i=e.wheelDeltaY||0;return a||i||(i=e.wheelDelta||0),!v.touchpadSupport&&f(i)?!0:(Math.abs(a)>1.2&&(a*=v.stepSize/120),Math.abs(i)>1.2&&(i*=v.stepSize/120),o(r,-a,-i),void e.preventDefault())}function r(e){var t=e.target,n=e.ctrlKey||e.altKey||e.metaKey||e.shiftKey&&e.keyCode!==H.spacebar;if(/input|textarea|select|embed/i.test(t.nodeName)||t.isContentEditable||e.defaultPrevented||n)return!0;if(s(t,"button")&&e.keyCode===H.spacebar)return!0;var r,a=0,i=0,u=l(w),c=u.clientHeight;switch(u==document.body&&(c=window.innerHeight),e.keyCode){case H.up:i=-v.arrowScroll;break;case H.down:i=v.arrowScroll;break;case H.spacebar:r=e.shiftKey?1:-1,i=-r*c*.9;break;case H.pageup:i=.9*-c;break;case H.pagedown:i=.9*c;break;case H.home:i=-u.scrollTop;break;case H.end:var d=u.scrollHeight-u.scrollTop-c;i=d>0?d+10:0;break;case H.left:a=-v.arrowScroll;break;case H.right:a=v.arrowScroll;break;default:return!0}o(u,a,i),e.preventDefault()}function a(e){w=e.target}function i(e,t){for(var o=e.length;o--;)z[N(e[o])]=t;return t}function l(e){var t=[],o=S.scrollHeight;do{var n=z[N(e)];if(n)return i(t,n);if(t.push(e),o===e.scrollHeight){if(!y||S.clientHeight+10<o)return i(t,document.body)}else if(e.clientHeight+10<e.scrollHeight&&(overflow=getComputedStyle(e,"").getPropertyValue("overflow-y"),"scroll"===overflow||"auto"===overflow))return i(t,e)}while(e=e.parentNode)}function u(e,t,o){window.addEventListener(e,t,o||!1)}function c(e,t,o){window.removeEventListener(e,t,o||!1)}function s(e,t){return(e.nodeName||"").toLowerCase()===t.toLowerCase()}function d(e,t){e=e>0?1:-1,t=t>0?1:-1,(k.x!==e||k.y!==t)&&(k.x=e,k.y=t,M=[],C=0)}function f(e){if(e){e=Math.abs(e),D.push(e),D.shift(),clearTimeout(A);var t=D[0]==D[1]&&D[1]==D[2],o=h(D[0],120)&&h(D[1],120)&&h(D[2],120);return!(t||o)}}function h(e,t){return Math.floor(e/t)==e/t}function m(e){var t,o,n;return e*=v.pulseScale,1>e?t=e-(1-Math.exp(-e)):(o=Math.exp(-1),e-=1,n=1-Math.exp(-e),t=o+n*(1-o)),t*v.pulseNormalize}function p(e){return e>=1?1:0>=e?0:(1==v.pulseNormalize&&(v.pulseNormalize/=m(1)),m(e))}var w,g={frameRate:150,animationTime:800,stepSize:120,pulseAlgorithm:!0,pulseScale:8,pulseNormalize:1,accelerationDelta:20,accelerationMax:1,keyboardSupport:!0,arrowScroll:50,touchpadSupport:!0,fixedBackground:!0,excluded:""},v=g,b=!1,y=!1,k={x:0,y:0},x=!1,S=document.documentElement,D=[120,120,120],H={left:37,up:38,right:39,down:40,spacebar:32,pageup:33,pagedown:34,end:35,home:36},v=g,M=[],T=!1,C=+new Date,z={};setInterval(function(){z={}},1e4);var A,N=function(){var e=0;return function(t){return t.uniqueID||(t.uniqueID=e++)}}(),E=function(){return window.requestAnimationFrame||window.webkitRequestAnimationFrame||function(e,t,o){window.setTimeout(e,o||1e3/60)}}(),K=/chrome/i.test(window.navigator.userAgent),L="onmousewheel"in document;L&&K&&(u("mousedown",a),u("mousewheel",n),u("load",t))}();
//]]></script>
<script>
//<![CDATA[
$(document).ready(function(){function relatedPost(g,e,r){$.ajax({url:"/feeds/posts/default/-/"+e+"?alt=json-in-script&max-results="+r,type:"get",dataType:"jsonp",success:function(t){for(var u="",h='<div class="related">',x=0;x<t.feed.entry.length;x++){for(var z=0;z<t.feed.entry[x].link.length;z++){if("alternate"==t.feed.entry[x].link[z].rel){u=t.feed.entry[x].link[z].href;break}}
var p=t.feed.entry[x].title.$t;var c=t.feed.entry[x].content.$t;var y=$('<div>').html(c);if(c.indexOf("http://www.youtube.com/embed/")>-1||c.indexOf("https://www.youtube.com/embed/")>-1){var d=t.feed.entry[x].media$thumbnail.url,m=d.replace('/default.jpg','/mqdefault.jpg'),k=m;}else if(c.indexOf("<img")>-1){var s=y.find('img:first').attr('src'),v=s.replace('s72-c','s600');var k=v;}else{var k='http://1.bp.blogspot.com/-eAeO-DYJDws/Vkqtj4HFBFI/AAAAAAAAB0o/Q5OLsyONXM0/s1600-r/nth.png';}
h+='<li><div class="related-thumb"><a class="related-img" href="'+u+'" style="background:url('+k+') no-repeat center center;background-size: cover"/></div><h3 class="related-title"><a href="'+u+'">'+p+'</a></h3></li>'}
h+='</div>',g.html(h);}})}
$("#related-posts").each(function(){var g=$(this),e=g.text(),r=3;relatedPost(g,e,r);});});
 //]]>
</script>

<script type='text/javascript'>
 /*<![CDATA[*/
$(window).bind("load", function () {
    jQuery("#loader").fadeOut("slow");
    jQuery("#preloader").delay(0).fadeOut();
});
  /*]]>*/
</script>
</body>
</html>
