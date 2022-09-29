# Modern CSS Initialize

CSS has evolved a lot in the past few years, and the main reason is the arrival of responsive design. For those unfamiliar with responsive design, responsive design is the process of designing websites that respond to different devices in order to provide the best user experience. With the arrival of CSS3, we got a lot of amazing features that enabled us to create responsive websites a lot easier with less code. In this post, we will cover some interesting features from CSS3, best practices for writing styles for your application, and cool tips for making your CSS better.

As mentioned above we want our website to work on all devices. The first issue we will face while creating a modern responsive website is inconsistent User Agent Styles. Let me explain, basically each browser comes with predefined styles for elements like h1 and p tag and they are not always the same (especially in IE). To solve this problem we have two options. The first and more aggressive approach is Reset CSS which will remove all User Agent Styles so that we can define them ourselves in our project. There are several good Reset.css implementations around, and it is not very hard to create your own. 


```
html {box-sizing: border-box;}
*, *::before, *::after {box-sizing: inherit;}
h1, h2, h3, h4, h5, h6{margin:0; font-size:inherit; font-weight:inherit;}
p{margin:0;}
a{text-decoration:none; color:inherit; cursor:pointer;}
button{background-color:transparent; color:inherit; border-width:0; padding:0; cursor:pointer;}
input::-moz-focus-inner {border:0; padding:0; margin:0;}
input, textarea {outline: 0;}
ul, ol, dd{margin:0; padding:0; list-style:none;}
cite {font-style:normal;}
fieldset{border-width:0; padding:0; margin:0;}
figure{margin:0;}
```
