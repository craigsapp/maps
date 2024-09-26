---
title: XYZ Tiles
layout: default
description: Explanation of the concept of tiles for mapping.
permalink: /tiles.html
---

{% include_relative styles-local.html %}

# Tiles


Choose a map tile server:

<select id="server-select" onchange="displayZoomTable()">
<option value="https://tile.openstreetmap.org/{z}/{x}/{y}.png">https://tile.openstreetmap.org/{z}/{x}/{y}.png</option>
<option value="https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}">https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}</option>
</select>


Choose zoom level: <select id="zoom-select" onchange="displayZoomTable(this)">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
    <option value="4">4</option>
</select>

<div id="tile-table">   </div>

<p>
<a target="_blank" href="https://en.wikipedia.org/wiki/Mercator_projection">Mercator projection</a>
</p>

<div style="height:50px;"></div>

## Example zooming in on a fixed coordinate:

Note that all tiles have the same dimension of 256&times;256 pixels.

Here is a list of tiles at each zoom level containing Warsaw (52.23 N, 21.011111 W) from z=0 (entire world) to z=19 (maximum zoom-in for OSM):

<p>

<table id="zoom">
<tr><th>Zoom</th><th>X</th><th>Y</th><th>Image (click to open in new window)</th></tr>

<tr><td>0</td><td>0</td><td>0</td><td> <a href="https://tile.openstreetmap.org/0/0/0.png" target="_blank"><img src="https://tile.openstreetmap.org/0/0/0.png" title="https://tile.openstreetmap.org/0/0/0.png"></a> </td></tr>
<tr><td>1</td><td>1</td><td>0</td><td> <a href="https://tile.openstreetmap.org/1/1/0.png" target="_blank"><img src="https://tile.openstreetmap.org/1/1/0.png" title="https://tile.openstreetmap.org/1/1/0.png"></a> </td></tr>
<tr><td>2</td><td>2</td><td>1</td><td> <a href="https://tile.openstreetmap.org/2/2/1.png" target="_blank"><img src="https://tile.openstreetmap.org/2/2/1.png" title="https://tile.openstreetmap.org/2/2/1.png"></a> </td></tr>
<tr><td>3</td><td>4</td><td>2</td><td> <a href="https://tile.openstreetmap.org/3/4/2.png" target="_blank"><img src="https://tile.openstreetmap.org/3/4/2.png" title="https://tile.openstreetmap.org/3/4/2.png"></a> </td></tr>
<tr><td>4</td><td>8</td><td>5</td><td> <a href="https://tile.openstreetmap.org/4/8/5.png" target="_blank"><img src="https://tile.openstreetmap.org/4/8/5.png" title="https://tile.openstreetmap.org/4/8/5.png"></a> </td></tr>
<tr><td>5</td><td>17</td><td>10</td><td> <a href="https://tile.openstreetmap.org/5/17/10.png" target="_blank"><img src="https://tile.openstreetmap.org/5/17/10.png" title="https://tile.openstreetmap.org/5/17/10.png"></a> </td></tr>
<tr><td>6</td><td>35</td><td>21</td><td> <a href="https://tile.openstreetmap.org/6/35/21.png" target="_blank"><img src="https://tile.openstreetmap.org/6/35/21.png" title="https://tile.openstreetmap.org/6/35/21.png"></a> </td></tr>
<tr><td>7</td><td>71</td><td>42</td><td> <a href="https://tile.openstreetmap.org/7/71/42.png" target="_blank"><img src="https://tile.openstreetmap.org/7/71/42.png" title="https://tile.openstreetmap.org/7/71/42.png"></a> </td></tr>
<tr><td>8</td><td>142</td><td>84</td><td> <a href="https://tile.openstreetmap.org/8/142/84.png" target="_blank"><img src="https://tile.openstreetmap.org/8/142/84.png" title="https://tile.openstreetmap.org/8/142/84.png"></a> </td></tr>
<tr><td>9</td><td>285</td><td>168</td><td> <a href="https://tile.openstreetmap.org/9/285/168.png" target="_blank"><img src="https://tile.openstreetmap.org/9/285/168.png" title="https://tile.openstreetmap.org/9/285/168.png"></a> </td></tr>
<tr><td>10</td><td>571</td><td>337</td><td> <a href="https://tile.openstreetmap.org/10/571/337.png" target="_blank"><img src="https://tile.openstreetmap.org/10/571/337.png" title="https://tile.openstreetmap.org/10/571/337.png"></a> </td></tr>
<tr><td>11</td><td>1143</td><td>674</td><td> <a href="https://tile.openstreetmap.org/11/1143/674.png" target="_blank"><img src="https://tile.openstreetmap.org/11/1143/674.png" title="https://tile.openstreetmap.org/11/1143/674.png"></a> </td></tr>
<tr><td>12</td><td>2287</td><td>1348</td><td> <a href="https://tile.openstreetmap.org/12/2287/1348.png" target="_blank"><img src="https://tile.openstreetmap.org/12/2287/1348.png" title="https://tile.openstreetmap.org/12/2287/1348.png"></a> </td></tr>
<tr><td>13</td><td>4574</td><td>2697</td><td> <a href="https://tile.openstreetmap.org/13/4574/2697.png" target="_blank"><img src="https://tile.openstreetmap.org/13/4574/2697.png" title="https://tile.openstreetmap.org/13/4574/2697.png"></a> </td></tr>
<tr><td>14</td><td>9148</td><td>5394</td><td> <a href="https://tile.openstreetmap.org/14/9148/5394.png" target="_blank"><img src="https://tile.openstreetmap.org/14/9148/5394.png" title="https://tile.openstreetmap.org/14/9148/5394.png"></a> </td></tr>
<tr><td>15</td><td>18296</td><td>10789</td><td> <a href="https://tile.openstreetmap.org/15/18296/10789.png" target="_blank"><img src="https://tile.openstreetmap.org/15/18296/10789.png" title="https://tile.openstreetmap.org/15/18296/10789.png"></a> </td></tr>
<tr><td>16</td><td>36593</td><td>21579</td><td> <a href="https://tile.openstreetmap.org/16/36593/21579.png" target="_blank"><img src="https://tile.openstreetmap.org/16/36593/21579.png" title="https://tile.openstreetmap.org/16/36593/21579.png"></a> </td></tr>
<tr><td>17</td><td>73186</td><td>43158</td><td> <a href="https://tile.openstreetmap.org/17/73186/43158.png" target="_blank"><img src="https://tile.openstreetmap.org/17/73186/43158.png" title="https://tile.openstreetmap.org/17/73186/43158.png"></a> </td></tr>
<tr><td>18</td><td>146372</td><td>86317</td><td> <a href="https://tile.openstreetmap.org/18/146372/86317.png" target="_blank"><img src="https://tile.openstreetmap.org/18/146372/86317.png" title="https://tile.openstreetmap.org/18/146372/86317.png"></a> </td></tr>
<tr><td>19</td><td>292745</td><td>172635</td><td> <a href="https://tile.openstreetmap.org/19/292745/172635.png" target="_blank"><img src="https://tile.openstreetmap.org/19/292745/172635.png" title="https://tile.openstreetmap.org/19/292745/172635.png"></a> </td></tr>


</table>

</p>



<script>

document.addEventListener("DOMContentLoaded", function () {
    let selectElement = document.querySelector("select#zoom-select");
    if (selectElement) {
        displayZoomTable(selectElement);
    }
});


function displayZoomTable(selectElement) {
    if (!selectElement) {
        selectElement = document.querySelector("#zoom-select");
    }
    let serverElement = document.querySelector("#server-select");
	let zoom = parseInt(selectElement.value);

	let output = `<table class="tile">\n`;

	for (let row=0; row <= (2 ** zoom ); row++) {
		output += "<tr>";
		if (row == 0) {
			for (let col=0; col <= (2 ** zoom); col++) {
				if (col == 0) {
					output += `<td></td>`;
				} else if (col == 1) {
					output += `<td class="top-row">x=0</td>`;
				} else {
					output += `<td class="top-row">${col-1}</td>`;
				}
			}
		} else { // row > 0
			for (let col=0; col <= (2 ** zoom); col++) {
				if (col == 0) {
					if (row == 1) {
						output += `<td class="narrow">y=0</td>`;
					} else {
						output += `<td class="narrow">${row-1}</td>`;
					}
				} else { // col > 0
                    let url = serverElement.value;
                    url = url.replace(/\{z\}/g, zoom);
                    url = url.replace(/\{x\}/g, col-1);
                    url = url.replace(/\{y\}/g, row-1);
					// let url = `https://tile.openstreetmap.org/${zoom}/${col-1}/${row-1}.png`;
					output += `<td class="tile"><a href="${url}" target="_blank"><img src="${url}" title="${url}"/></a></td>`;
				}
			}
		}
		output += "</tr>\n";
	}

    output += "</table>";

	let tableElement = document.querySelector("#tile-table");
	tableElement.innerHTML = output;

}


</script>


