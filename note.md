# important notes

## diffrence between width and max width

- In CSS, the width property is used to set the width of an element. The max-width property is used to set the maximum width of an element. When you set the width property, it will prevent the element from stretching out to the edges of its container. On the other hand, when you use max-width, it will improve the browser’s handling of small windows. This is important when making a site usable on small devices

- max width doesn't creat a horizontal scroll bar but width create a horizontal scroll bar

## rem

- In CSS, rem stands for “root em”. It is a relative unit of measurement based on the font size of the root element, often the HTML element. Unlike pixels, which are absolute units independent of the viewport, rem units are flexible, enabling scalable elements and responsive design.

- rem unit is: "Equal to the computed value of font-size on the root element. When specified on the font-size property of the root element, the rem units refer to the property’s initial value"

- rem unit is related to the font size of the html element .. in generally the font size of the html element is
  16px so the 1 rem = 16px but we can change the size of the html element example if the html element font size is 10px then 1 rem = 10 px .... this provide the flexibility to the layout
- but if the user changes its original size on its browser than it can't inherit it and it produces chaos in our layout so for removing that we use percentage like 10/16 == 0.625 -> 62.5% this make font size of the html element to 10 px

## not pseudo-class

.grid:not(:last-child){
margin-bottom: 9.6rem;
}

in this is said that the grid that is not a last child then it have a magin bottom of 9.6rem

## Media Query

syntax:-

@media(max-width:1200px){
.section-hero{
background-color:red;
}
}

here above example if the screen size is less than the 1200px then the css applied inside it

# note :- media query simply work like a css priority its mean that the css come later is applied

## choosing element on the basis of the any attribute name

example:
<ion-icon name="menu-outline" class="icon-mobile-nav"></ion-icon>
<ion-icon name="close-outline" class="icon-mobile-nav"></ion-icon>

.icon-mobile-nav[name="close-outline"] {
display: none;
}

above example mean choose the element on the basic on name attribute which has a value of close-outline

## scroll - behaviour

scroll-behavior: smooth;

## webkit

we add webkit because is site "caniuse.com" according to this site backdrop not working on the safari and we can use webkit prefix to fix it
