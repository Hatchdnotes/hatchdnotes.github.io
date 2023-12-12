---
created: 2023-12-11T17:40:54-07:00
modified: 2023-12-11T17:57:44-07:00
---

# Web framework

***Testing a "Web Framework" using around 20 lines of code or less***

---

# HTML

---
 
``` html

<div class="hbox">
       <button>do</button>
       <button>stuff</button>
       <button>left</button>
       <span class="grow"></span>
       <b>Your CSS Framework </b>  
       <span class="grow"></span>
       <button class="fa fa-cut"></button>
       <button class="fa fa-copy"></button>
       <button class="fa fa-paste"></button>
   </div>

<div class="vbox panel" id="sources">
           <div class="header">Sources</div>
           <div class="scroll">
               <ul>
                   <li>list item </li>
                   <li>list item </li>
                   <li>list item </li>
                   <li>list item </li>
                 ….
           </div>
       </div>

```

# CSS

---

``` CSS 

@import "node_modules/font-awesome/css/font-awesome.css";
@import "node_modules/@typopro/web-source-sans-pro/TypoPRO-SourceSansPro.css";
@import "node_modules/@typopro/web-source-code-pro/TypoPRO-SourceCodePro.css";
@import "node_modules/@typopro/web-source-serif-pro/TypoPRO-SourceSerifPro.css";
body, button, input, select {  font-family: 'TypoPRO Source Sans Pro'; font-size: 100%; line-height: 140%; }
pre, code { font-family: 'TypoPRO Source Code Pro';  }

.hbox, .vbox { display: flex; }
.hbox { flex-direction: row; }
.vbox { flex-direction: column; }

.grow { flex: 1;  }

scroll { overflow: auto; }
.fill { position: absolute; top: 0; bottom: 0; left: 0; right:0; }

```

# JavaScript 

---

``` JavaScript

function $(selector) { return document.querySelector(selector);  }
function $$(selector) { return document.querySelectorAll(selector); }
$("#someid"); //fetch the element with the id ‘someid’

function printHello() {
   console.log("Hello!")
}
$$("button").forEach(button => button.addEventListener('click', printHello));

```
