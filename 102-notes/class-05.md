# Class 05

## CSS

This made much more sense after 101:  
+ Using tag, id, class make sense now. CSS selectors are familiar from web-scraping but their purpose makes sense
+ CSS syntax has tagname or #id or .classname for selectors, and more options and ways to be specific in selecting elements
+ This makes sense of commands like getElementById, getElementsByClassName, getElementByTagName in js and in webscraping with python
+ I can see myself spending a lot of time searching for how to achieve things with css and tryign to understand the ways solutions have been hacked together
+ I will have to think about what browsers might use things I write, and choose css accordingly - not everything is supported - eg [compatible fonts](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family#browser_compatibility)  

TIL:   
+ ! and tab gets a load of html set up by VSCode
+ *display: block* is default - block means full line occupied; *inline* means an element can share the line with other elements - like wrap text round image in Word etc. Ironically, for img the default is inline, and this mean it doesn't respond to margins - it needs to be inline-block
+ Definitely __write your html before your css__
+ Link to CSS like this and don't forget the rel=   
```
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
```

+ Also 
``` 
    <img src="">
    <link href="">
    <a href="">
```
It makes sense but I muddled them today

+ Note: Do not add a space between the property value and the unit:
Incorrect (space): margin-left: 20 px;   
Correct (nospace): margin-left: 20px;   
+ Specificity   
>inline styles added to an element  always overwrite styles defined in the head section of the document, which overwrite styles defined in external stylesheets. Here’s an easy way to remember this: whatever style of CSS is closest to the HTML is considered more relevant by browsers and will therefore be applied. This hierarchy is known as CSS specificity.
[https://blog.hubspot.com/website/add-css-to-html#:~:text=Using%20internal%20CSS%20is%20considered,elements%20over%20and%20over%20again]
+  if the style will be applied to multiple objects, it's wise to follow "Don't Repeat Yourself" (DRY) and assign it to a CSS class to be referenced by each element.   
+ Should I use inline, internal or external CSS? a stack overflow response says: 
>I think that inline styles are lazy. I say this because I do it so often myself, so I know -why- I'm doing it, because I have no idea whether the style will stay, so I used to do it right next to the html. These days, with html5 and pragmatic support for *style* anywhere, I use a nearby *style* tag instead while messing with layout, and then migrate it to the core/main css file after. Same benefits of speed and immediacy, almost none of the disadvantages (side effects on off-page elements due to specificity being one). – Kzqai Nov 22,   

Also from that question:
The advantage for having a different css file are

1. Easy to maintain your html page
2. Change to the Look and feel will be easy and you can have support for many themes on your pages.
3. Your css file will be cached on the browser side. So you will contribute a little on internet traffic by not loading some kbs of data every time a the page is refreshed or user navigates your site. *m3kh answered Apr 10, 2010 at 6:30*
