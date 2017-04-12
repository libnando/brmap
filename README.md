BrMap
======

#### Map of Brazil (html5, svg, js) - Interactive map for data visualizations. Bundled into a single Javascript file.

Intended to provide some data visualizations based on geographical data. It's SVG-based, can scale to any screen size.

* Mapa do Brasil (HTML5, SVG, js) - mapa interativo para visualização de dados. Empacotado em um único arquivo Javascript.

---

### Getting Started

1. Include 'brmap.js' on your page.
2. Create a BrMap object, passing at least the parameter 'wrapper'.

Example:
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<title>Brazil SVG</title>
</head>
<body>
	
	<div style="width: 600px;">
		<div id="br_mine"></div>
	</div>
	
	<script type="text/javascript" src="brmap.js"></script>
	<script type="text/javascript">
		new BrMap({
			wrapper: '#br_mine', 
			selectStates: ['sc'],
			callbacks: {
				click: function (element, uf) { alert(uf); },
				mouseover: function (element, uf){ console.log(uf); },
			}
		});
	</script>

</body>
</html>
```

---

#### Default Options
```js
  {
   wrapper: null,
		selectStates: [],
		cssFill: {
			shape: "#D8D6D6",
			icon_state: "#BBBBBB",
			label_icon_state: "#777777",
			label_state: "#FFFFFF",
			selected: "#BBBBBB"
		},
		responsive: true,
		width: 500,
		callbacks: {
			click: function (element, uf) { },
			mouseover: function (element, uf) { }
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
