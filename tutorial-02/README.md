<!-- Output copied to clipboard! -->

<!-----

You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 22

Conversion time: 5.259 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β34
* Wed Sep 27 2023 07:05:18 GMT-0700 (PDT)
* Source doc: Responsive design with CSS Guide
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server. NOTE: Images in exported zip file from Google Docs may not appear in  the same order as they do in your doc. Please check the images!

----->

# Simple Life - a demo responsive website.

<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 0; ALERTS: 22.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>
<a href="#gdcalert13">alert13</a>
<a href="#gdcalert14">alert14</a>
<a href="#gdcalert15">alert15</a>
<a href="#gdcalert16">alert16</a>
<a href="#gdcalert17">alert17</a>
<a href="#gdcalert18">alert18</a>
<a href="#gdcalert19">alert19</a>
<a href="#gdcalert20">alert20</a>
<a href="#gdcalert21">alert21</a>
<a href="#gdcalert22">alert22</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>

# Outline

[TOC]

## Choosing the Right Unit for the Right Task

### Percentage

Percentage as a unit value is usually relative to the parent element size. For example, if we add CSS of the div width as 50% and then write another div inside the first div and add CSS for the second div width as 50%. Then the first one is the parent of the second one and in this case, the second one’s width will be 50% compared to the first div.

&lt;div class=”first”>

    &lt;div class=”second”>

&lt;/div>

&lt;/div>

**<span style="text-decoration:underline;">Style.css:</span>**

.first{

width:50%; //50% of the root display size, for example 1450x50%=725

}

.second{

width:50%; //50% of its parent first div’s width, that will be 725x50%=362.5

}

#### Drawbacks

- Compounding Effect: Trouble in Paradise

### Em unit

It is almost similar to the percentage unit, em is borrowed from the [typography world](<https://en.wikipedia.org/wiki/Em_(typography)>), and it’s a unit that allows setting the font size of an element relative to the font size of its parent. (**Remember**): **when em units are used on font size, the size is relative to the font size of the parent. When used on other properties, it's relative to the font size of the element itself.**

**Source: [rem vs em Units in CSS | DigitalOcean](https://www.digitalocean.com/community/tutorials/css-rem-vs-em-units#rem-unit)**

#### Drawbacks

- [Compounding Effect: Trouble in Paradise](https://www.digitalocean.com/community/tutorials/css-rem-vs-em-units#compounding-effect-trouble-in-paradise)

### Rem unit

The rem unit, short for root em is a relative unit that’ll always be based upon the font-size value of the root element, which is the &lt;html> element. And if the &lt;html> element doesn’t have a specified font-size, the browser default of 16px is used.

So that means that by using the rem unit, the values of parent elements are ignored, and only the value of the root is taken into consideration.

### How to decide which unit to use?

#### A general rule of thumb:

- Font-size = rem
- Padding and margin = em
- Widths = em or percentage

##### How they work: A demonstration [36:00](https://youtu.be/srvUrASNj0s?si=qWKAzU7_sXFKsOUA&t=2162) and ems vs rems

We are going to utilize one character of em, **When em is used on other properties than font-size (padding, margin), it's relative to the font size of the element itself.**

Here when **px **is used in padding it does not adjust considering the font size of the element, look at the padding length on the left side for contact me, and about me remains almost the same.

<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image1.png "image_tooltip")

But with **em **as the unit, this will be solved, cause it will adjust based on the font-size of itself. See below now about me’s left size padding seems appropriate based on its’s font-size, not so big as before.

<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image2.png "image_tooltip")

## Flexbox

### The basics of Flexbox

Elements normally have a display: block or a display: inline as a

default from the browser.

#### Block elements (by default)

Block elements stack on top of each other

- div, header, footer, main, etc.
- h1 -> h6
- p

#### Inline elements (by default)

Inline elements stay within the flow of what's around them

- a
  - &lt;p>please, &lt;a href=”#”>click me&lt;/a> for more update&lt;p>
  - This anchor tag will remain inline.
- strong
- em
- Span

### Designing with flexbox

<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image3.png "image_tooltip")

We will design the following to understand how flexbox works.

<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image4.png "image_tooltip")

<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image5.png "image_tooltip")

#### Flexbox Justify content:

#### Flexbox Align items:

<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image6.png "image_tooltip")

Default: stretch

<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image7.png "image_tooltip")

<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image8.png "image_tooltip")

<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image9.png "image_tooltip")

<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image10.png "image_tooltip")

```
align-items: baseline;
/*Is not used much*/
```

#### Applying media queries [11:16:38](https://youtu.be/srvUrASNj0s?si=twWL5QBYwfbZQesn&t=4598)

Media queries let us add new styles that target only specific conditions

Media queries - basic syntax

@media media-type and (media-features) { ... }

media-type and media-features are optional. But you have to have one of them.

Media queries - media type

The media type lets us target different

types of media

- Screen @media screen {...}
- Print @media print {...}
- Speech @media speech {...}

Media queries - media condition

The media condition lets us target specific conditions within that media type

- Widths @media (min-width: 600px) {...}
- Orientation @media (orientation: landscape) {...}
- Specific features @media (hover) {...}

#### flex-direction

_flex-direction: row_; is by default.

<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image11.png "image_tooltip")

Earlier justify-content was working for spacing between rows,

<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image12.png "image_tooltip")

Now, it will work for the columns when we set _flex-direction: column._

<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image13.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image13.png "image_tooltip")

**Remember**,

justify-content will always work on the main axis.

align-items will now work on the cross-axis.

<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image14.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image14.png "image_tooltip")

<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image15.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image15.png "image_tooltip")

Also combining items as well.

<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image16.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image16.png "image_tooltip")

## Media Queries Basic

Media queries let us add new styles that target only specific conditions

Media queries - basic syntax

@media media-type and (media-features) { ... }

media-type and media-features are optional. But you have to have one of them.

Media queries - media type

The media type lets us target different

types of media

- Screen @media screen {...}
- Print @media print {...}
- Speech @media speech {...}

Media queries - media condition

The media condition lets us target specific conditions within that media type

- Widths @media (min-width: 600px) {...}
- Orientation @media (orientation: landscape) {...}
- Specific features @media (hover) {...}
-

### How to choose the media query break-point?

Media query break-point is layout-specific. Since there are tons of devices out there with different sizes, it is hard to cover everything. Thus it is better to have a break-point according to your layout. If your layout breaks or looks ugly at a certain point this is the point where you should add a break-point. May be 675px is good, maybe something else, it all depends on the how the layout reacts,

#### @media (min-width: 675px) {...}

## Responsive Navigation

<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image17.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image17.png "image_tooltip")

Living the simple life

A BLOG EXPLORING MINIMALISM IN LIFE

HOME | ABOUT ME | RECENT POSTS

**Colors:**

#F8F8F8

#707070

#1792D2

#143774

**Font-size:**

Title: Lora 3.375rem

Subtitle: Ubuntu bold - 1 rem

Navigation: Ubuntu bold - 1rem

**Font size (Maybe for Mobile first):**

Title: Lora 2rem

Subtitle: Ubuntu bold - 0.75rem

Navigation: Ubuntu bold - 1rem

Bold ~= 700 font-weight.

[Navi](https://youtu.be/srvUrASNj0s?si=xpdXCHKeE5E-5tkZ&t=5809)

Navigation Version 2: pink lines indicate the layout.

So far, we have the outermost &lt;header> container for containing all of these. Additionally, we have the &lt;div> for containing the site title and subtitle. Also, we have the &lt;nav> for containing the nav links. We don't have the container containing these two things. We need a container here.

<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image18.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image18.png "image_tooltip")

Navigation Version 3: for mobile-friendly

<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image19.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image19.png "image_tooltip")

## A complete responsive website project

[Living the simple life (adobe.com)](https://xd.adobe.com/spec/75d448ea-569a-4b7e-721b-9bbd3b2b97b9-03e5/screen/c27ed1eb-3c57-41a8-acb2-90ecaf25f93b/specs/)

<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image20.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image20.png "image_tooltip")

<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image21.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image21.png "image_tooltip")

#F8F8F8

#707070

#1792D2

#143774

Font weights:

1. Light - 300
2. Regular/Normal - 400
3. Medium - 500
4. SemiBold - 600
5. Bold - 500

Lora (400 font-weight) 2rem Living the simple life

Lora (400 font-weight) 1.5rem Heading 2 (blog post titles)

Lora 1.125rem Heading 3 (blog post titles)

Ubuntu bold .75rem **SUBHEADING**

Ubuntu light 1.125rem body text

Ubuntu bold 0.875rem **CONTINUE READING**

Ubuntu light 0.875rem Dates

---

Part 2

Widget title

Ubuntu bold 1rem **ABOUT ME**

Ubuntu Light 1rem Keep Cooking Simple

<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image22.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image22.png "image_tooltip")

### Order

Note: You can use order only if you make the display property flex. Otherwise, the order will not work.

### Viewport metatag

Sometimes what happens is your mobile device or other device might tell the browser that it is 960px but actually they are 360px. When the browser treats it as 960px instead of 360px, it will try to render a website that is ideal for a 960px device, as a result inside a 360px device we will experience a zoomed-out version of our website. To prevent the browser from rendering a zoomed-out version, we can add a metatag like the following,

```
<meta name="viewport" content="width=device-width, initial-scale=1" />
```

With this tag added, even if the device sends a wrong device size to the browser, this tag will readjust the zoomed-out site to shrink and display it accordingly. This `width=device-width `will enable the browser to readjust the width thus the device size. And this `initial-scale=1 `will make sure the zoom scale is 100% (1 is equivalent to 100%).
