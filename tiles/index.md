---
title: XYZ Tiles
layout: default
description: Explanation of the concept of tiles for mapping.
permalink: /tiles.html
---

{% include_relative styles-local.html %}

https://tile.openstreetmap.org/{z}/{x}/{y}.png


<select id="zoom-select" onchange="displayZoomTable(this)">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
    <option value="4">4</option>
</select>


<div id="tile-table">   </div>


# Example zooming in on a fixed coordinate:

Tiles containing Warsaw at various zoom levels from 0 (entire world) to 19 (maximum zoom for OSM):

<p>

<table>
<tr><th>Zoom</th><th>Image (click to open in new window)</th></tr>

<tr><td>0</td><td> <a href="https://tile.openstreetmap.org/0/0/0.png" target="_blank"><img src="https://tile.openstreetmap.org/0/0/0.png" title="https://tile.openstreetmap.org/0/0/0.png"></a> </td></tr>
<tr><td>1</td><td> <a href="https://tile.openstreetmap.org/1/1/0.png" target="_blank"><img src="https://tile.openstreetmap.org/1/1/0.png" title="https://tile.openstreetmap.org/1/1/0.png"></a> </td></tr>
<tr><td>2</td><td> <a href="https://tile.openstreetmap.org/2/2/1.png" target="_blank"><img src="https://tile.openstreetmap.org/2/2/1.png" title="https://tile.openstreetmap.org/2/2/1.png"></a> </td></tr>
<tr><td>3</td><td> <a href="https://tile.openstreetmap.org/3/4/2.png" target="_blank"><img src="https://tile.openstreetmap.org/3/4/2.png" title="https://tile.openstreetmap.org/3/4/2.png"></a> </td></tr>
<tr><td>4</td><td> <a href="https://tile.openstreetmap.org/4/8/5.png" target="_blank"><img src="https://tile.openstreetmap.org/4/8/5.png" title="https://tile.openstreetmap.org/4/8/5.png"></a> </td></tr>
<tr><td>5</td><td> <a href="https://tile.openstreetmap.org/5/17/10.png" target="_blank"><img src="https://tile.openstreetmap.org/5/17/10.png" title="https://tile.openstreetmap.org/5/17/10.png"></a> </td></tr>
<tr><td>6</td><td> <a href="https://tile.openstreetmap.org/6/35/21.png" target="_blank"><img src="https://tile.openstreetmap.org/6/35/21.png" title="https://tile.openstreetmap.org/6/35/21.png"></a> </td></tr>
<tr><td>7</td><td> <a href="https://tile.openstreetmap.org/7/71/42.png" target="_blank"><img src="https://tile.openstreetmap.org/7/71/42.png" title="https://tile.openstreetmap.org/7/71/42.png"></a> </td></tr>
<tr><td>8</td><td> <a href="https://tile.openstreetmap.org/8/142/84.png" target="_blank"><img src="https://tile.openstreetmap.org/8/142/84.png" title="https://tile.openstreetmap.org/8/142/84.png"></a> </td></tr>
<tr><td>9</td><td> <a href="https://tile.openstreetmap.org/9/285/168.png" target="_blank"><img src="https://tile.openstreetmap.org/9/285/168.png" title="https://tile.openstreetmap.org/9/285/168.png"></a> </td></tr>
<tr><td>10</td><td> <a href="https://tile.openstreetmap.org/10/571/337.png" target="_blank"><img src="https://tile.openstreetmap.org/10/571/337.png" title="https://tile.openstreetmap.org/10/571/337.png"></a> </td></tr>
<tr><td>11</td><td> <a href="https://tile.openstreetmap.org/11/1143/674.png" target="_blank"><img src="https://tile.openstreetmap.org/11/1143/674.png" title="https://tile.openstreetmap.org/11/1143/674.png"></a> </td></tr>
<tr><td>12</td><td> <a href="https://tile.openstreetmap.org/12/2287/1348.png" target="_blank"><img src="https://tile.openstreetmap.org/12/2287/1348.png" title="https://tile.openstreetmap.org/12/2287/1348.png"></a> </td></tr>
<tr><td>13</td><td> <a href="https://tile.openstreetmap.org/13/4574/2697.png" target="_blank"><img src="https://tile.openstreetmap.org/13/4574/2697.png" title="https://tile.openstreetmap.org/13/4574/2697.png"></a> </td></tr>
<tr><td>14</td><td> <a href="https://tile.openstreetmap.org/14/9148/5394.png" target="_blank"><img src="https://tile.openstreetmap.org/14/9148/5394.png" title="https://tile.openstreetmap.org/14/9148/5394.png"></a> </td></tr>
<tr><td>15</td><td> <a href="https://tile.openstreetmap.org/15/18296/10789.png" target="_blank"><img src="https://tile.openstreetmap.org/15/18296/10789.png" title="https://tile.openstreetmap.org/15/18296/10789.png"></a> </td></tr>
<tr><td>16</td><td> <a href="https://tile.openstreetmap.org/16/36593/21579.png" target="_blank"><img src="https://tile.openstreetmap.org/16/36593/21579.png" title="https://tile.openstreetmap.org/16/36593/21579.png"></a> </td></tr>
<tr><td>17</td><td> <a href="https://tile.openstreetmap.org/17/73186/43158.png" target="_blank"><img src="https://tile.openstreetmap.org/17/73186/43158.png" title="https://tile.openstreetmap.org/17/73186/43158.png"></a> </td></tr>
<tr><td>18</td><td> <a href="https://tile.openstreetmap.org/18/146372/86317.png" target="_blank"><img src="https://tile.openstreetmap.org/18/146372/86317.png" title="https://tile.openstreetmap.org/18/146372/86317.png"></a> </td></tr>
<tr><td>19</td><td> <a href="https://tile.openstreetmap.org/19/292745/172635.png" target="_blank"><img src="https://tile.openstreetmap.org/19/292745/172635.png" title="https://tile.openstreetmap.org/19/292745/172635.png"></a> </td></tr>


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
	let zoom = parseInt(selectElement.value);

	let output = `<table class="tile">\n`;

	for (let row=0; row <= (2 ** zoom ); row++) {
		output += "<tr>";
		if (row == 0) {
			for (let col=0; col <= (2 ** zoom); col++) {
				if (col == 0) {
					output += `<td></td>`;
				} else if (col == 1) {
					output += `<td>x=0</td>`;
				} else {
					output += `<td>${col-1}</td>`;
				}
			}
		} else { // row > 0
			for (let col=0; col <= (2 ** zoom); col++) {
				if (col == 0) {
					if (row == 1) {
						output += `<td>y=0</td>`;
					} else {
						output += `<td>${row-1}</td>`;
					}
				} else { // col > 0
					let url = `https://tile.openstreetmap.org/${zoom}/${col-1}/${row-1}.png`;
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


