**Koala :**

Welcome to Koala.

Koala is a real minimal javascript framework for hybrid mobile aplications.

**History :**

I wrote koala.js for my hybrid mobile application in short time. You know, modern frameworks like jquery registers many events in dom. Effects, events and other some methods are uses high cpu and memory recources. If you are developing mobile apps based on cordova - phonegap, you have to optimize your apps memory and cpu usage. 

Koala works for simple actions(show,hide,select,fadeIn..) with low recource(cpu,memory) usage and not includes any other framework. 

Koala has very simple code and many lost features then other complex frameworks.  


**Functions :**

- get(query)           : single dom element (works with native dom selectors)
- getAll(query)        : return NodeList inculedes all elements for query (works with native dom selectors)
- show(target)         : show dom element (display:block)
- hide(target)         : hide dom element (display:none)
- fadeIn(target,delay) : show element with fadeIn effect
- fadeOut(target,delay): hide element with fadeOut effect
- inArray(arr,value)   : check given value is in given array


**Events:**
- click(target, Callback)             : set click listener for given dom element 
- event(eventname, target, Callback)  : set listener to given event for given dom element 


**Basic Usage:**

_Getting Single Element_

`koala.get("div#container");`

`koala.get("div#container a");`

`var elm = koala.get("div#container");`


_Getting All Elements For Query_

`koala.getAll("div a");`

`var elmNodeList = koala.getAll("div a");`


_Show Hidden Element_

`koala.show(elm);`


_Hide Element_

`koala.hide(elm);`


_Show element with fadeIn effect_

`koala.fadeIn(target, 300);`


_Hide element with fadeOut effect_

`koala.fadeOut(target, 300);`


_Search Value in Array_

`var arr = Array("banana","apple","pie","wine");`

`koala.inArray(arr, "wine");`


_Set Click Event_

`koala.click(elm, function({`
  `console.log("Koala Click");`
`}));`


_Set listener to given event for given dom element_

`koala.event("mousemove", elm, function(){ console.log("Koala Event") });`
