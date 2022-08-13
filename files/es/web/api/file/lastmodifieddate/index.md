---
title: File.lastModifiedDate
slug: Web/API/File/lastModifiedDate
tags:
  - API
  - Archivo
  - Archivos
  - Deprecado
  - File API
  - Propiedad
  - Referencia
  - Solo lectura
translation_of: Web/API/File/lastModifiedDate
---
<div>{{APIRef("File API") }} {{deprecated_header}}</div>

<p>La propiedad de solo lectura <code><strong>File.lastModifiedDate</strong></code><strong> </strong>retorna la fecha de ultima modificacion del archivo. Archivos sin una ultima fecha de modificacion conocida retornan la fecha actual.</p>

<h2 id="Sintaxis">Sintaxis</h2>

<pre class="brush: js">var time = <em>instanceOfFile</em>.lastModifiedDate</pre>

<h2 id="Valor">Valor</h2>

<p>Un objeto <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date">Date</a></code>.</p>

<h2 id="Ejemplo">Ejemplo</h2>

<pre class="brush:js">// fileInput es un HTMLInputElement: &lt;input type="file" multiple id="myfileinput"&gt;
var fileInput = document.getElementById("myfileinput");

// files es un objeto FileList (similar a NodeList)
var files = fileInput.files;

for (var i = 0; i &lt; files.length; i++) {
  alert(files[i].name + " tiene una fecha de ultima modificacion el " + files[i].lastModifiedDate);
}</pre>

<h2 id="Especificaciones">Especificaciones</h2>

<p><em>Aunque estaba presente en las primeras versiones de la especificacion de File API, esta propiedad ha sido eliminada de esta y ahora es no-estandar. Usar {{domxref("File.lastModified")}} como reemplazo.</em></p>

<h2 id="Compatibilidad_con_navegadores">Compatibilidad con navegadores</h2>

{{Compat("api.File.lastModifiedDate")}}

<h2 id="Vea_también">Vea también</h2>

<ul>
 <li>{{domxref("File")}}</li>
</ul>