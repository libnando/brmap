brMap
======

#### Map of Brazil (html5, svg, js) - Interactive map for data visualizations. Bundled into a single Javascript file.

Intended to provide some data visualizations based on geographical data. It's SVG-based, can scale to any screen size.

* Mapa do Brasil (HTML5, SVG, js) - mapa interativo para visualização de dados. Empacotado em um único arquivo Javascript.

---

### Getting Started

1. Include 'brmap.js' and 'brmap.css' on your page.
2. Create a brMap object, passing at least the parameter 'element'.

Example:
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<script src="brmap.js"></script>
<link href="brmap.css" rel="stylesheet" type="text/css">
<title>Brazil SVG</title>
</head>
<body>
	<div id="meumapa"></div>
	<script>
		brMap({	element: "#meumapa" });
		
		//specifying....
		
		/*		
		brMap({
			element: "#meumapa",
			cssClass : 'blue', //green, gray, blue, orange
			responsive: false,
			width:500,
			selectStates : ["go", "ac"],
			callbacks: {
				onClick	: function (element, uf){
             		console.log(uf);             		
            	}
             }
		});*/
		
	</script>
</body>
</html>
```

---

#### Default Options
```js
  {
    element : null, //required
	selectStates : [],
	cssClass : 'gray',
	responsive : true,
	width : 500, //case not responsive
	callbacks : {
		onMouseOver : function(element, uf){},
		onClick : function(element, uf){},
	}
  }
```
---

#### Browser support

<table width="100%" style="text-align: center;">
  <thead>
    <tr>
      <td>Safari</td>
      <td>Firefox</td>
      <td>Chrome</td>
      <td>IE8</td>
      <td>IE9</td>
      <td>IE10</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>✔</td>
      <td>✔</td>
      <td>✔</td>
      <td>✖†</td>
      <td>✔</td>
      <td>✔</td>
    </tr>
  </tbody>
</table>


#### Demos

 - [Default](http://bloosoft.com.br/os/brmap/default.html)
 - [Specific](http://bloosoft.com.br/os/brmap/specific.html)
