---
title: Computable Blocks of the Internet
layout: post
---

Web components aren’t enabling us to do something we were unable to do before, they’re simply a new tool that promote component-based software engineering in how we build web apps. The largest value to web components is that they promote expressivity, reusability and encapsulation. 

<div id='cover-image' style='width:650px;height:350px;position:relative; margin: 30px 0 30px -25px'>
<x-life width='650' height='350' backgroundColor = 'rgb(160,248,253)' cellColor='rgb(250,230,60)' cellSize = '3' >
</x-life>
	<div id='caption'>Check the code</div>

</div>

<!-- ![Alt text](/assets/gol.png)
 -->
<!-- <div id='cover'>

</div> -->
##Web Components


Web components are reusable components that encapsulate HTML, CSS and Javascript. To learn more about web components, I’d suggest reading the official <a href='http://w3c.github.io/webcomponents/explainer/'>w3c specification</a>, or watching Eric Bidelman's talk, <a href='https://www.youtube.com/watch?v=fqULJBBEVQE'>Web Components: A Tectonic Shift for Web Development</a>. In short, these components are built using the following four technologies :

<b>Templates</b> The <template\> tag allows you to define markup to be used later. 

<b>Custom templates </b> The custom elements specification allows developers to define their own DOM elements. 

<b>Shadow DOM</b> Encapsulate code so that it doesn’t bleed out into the external code.

<b>HTML Imports</b> I know what you’re thinking, <em>why doesn’t this exist yet</em>?

	<link rel="import" href="import.html">


##Component Based Web-Apps

Web components aren’t enabling us to do something we were unable to do before, they’re simply a new tool that promote component-based software engineering in how we build web apps. The largest value to web components is that they promote expressivity, reusability and encapsulation. 

<b>Expressive markup </b> Modern web components suffer from <div\> soup syndrom. Expressive markup  means writing web apps that are easier to read and maintain.  My favorite example of the potential expressivity web components promise is a <a href=" http://www.html5rocks.com/en/tutorials/webcomponents/customelements/">rewrite</a> of the GMAIL hangout module using Polymer, by Eric Bidelman.

<b>Encapsulation </b> Shadow DOM allows you to encapsulate code so that it doesn’t bleed out into the external code. This avoids component soup, but also prevents internal variables of the component, such as its styling, from mixing with the global scope. So any external style sheets or javascript has no effect on the component. 

<b>Reusability </b> Platforms such as <a href='http://component.kitchen/'>Component Kitchen</a> are already promoting the sharing of web components. Sharing web components, as an alternative to sharing raw javascript, html and css files and asking the developer to … Despite that, these components are still versatile. Configuring components can be done through an interface of attributes, methods and events. Because of the ease of plugging in and configuring these components, reusability is much easier. 


## X-Life
To start dabbling with Polymer, I built <a href='http://acrylc.github.io/x-life'><x-life\></a>, a web component for Conway's Game of Life. The component encapsulates a canvas object and the logic for Life. At intialization, a random configuration of cells is created and a new generation is computed every 100ms.

To try out <x-life\> :

<b>Install using bower</b>

	bower install x-life --save

<b>Import polymer and x-life</b>

	<script src="bower_components/platform/platform.js"> </script>
	<link rel='import' href="bower_components/x-life/dist/x-life.html"> 

<b>Include the x-life tag</b>

	<x-life> </x-life>
<br>

Attribute  | Options           | Default             | Description
---        | ---         | ---                 | ---
`width` | *int*   | 500             | Specifies the width of the GOL grid.
`height` | *int*   | 500            | Specifies the height of the GOL grid.
`backgroundColor` | *string*   | `white`             | Specifies the background color, in rgb or hex.
`cellColor` | *string*   | `black`             | Specifies the cell color, in rgb or hex.
`cellSize`     | *float*    |  2   | Specifies the pixel size of a cell.



## Computable Bits
As a web developer, I'm very excited about web components. 
When I first encountered web components, I was particularly fascinated by the illusion created by the shadow DOM's encapsulation of component code. Web components are simple markup after all, but can hide away the workings of a turing machine. Giving a markup language such power is going to ... 

I'm reminded of Little Bits, a library of of electronic pre-programmed modules that snap together with magnets. I wasn't able to build my first robot untill my first year in undergrad, but I'll never forget my fascination as I watched my cousin's 10 year old daughter snap together her first pair of Little Bits to build a robot whose eyes light up when you shake his hand. Similarly, these web components, with their promises of expressivity, encapsulation and reusabilty, can snap together and vastly amplify our abilities in building web applications.

