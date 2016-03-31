---
layout: page
title: SetHTMLFooterByName()
parent_title: mPDF functions
permalink: /reference/mpdf-functions/sethtmlfooterbyname.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>(mPDF &gt;= 2.0)</p>
<p>SetHTMLFooterByName – Sets an HTML page footer by a given name</p>
<h2>Description</h2>

<div class="alert alert-info" role="alert">void <b>SetHTMLFooterByName</b> ( string <span class="parameter">$name</span> [, string <span class="parameter">$side</span> ])</div>
<p>Sets an HTML page footer that has previously been defined by name.</p>

<div class="alert alert-info" role="alert"><b>Note: </b>This function/method was altered in mPDF 2.2 by capitalising the first letter of the name. As function/method names in PHP have hitherto been case-insensitive, this should not cause any problems, but it is recommended where possible to use the preferred spelling.</div>
<h2>Parameters</h2>
<p class="manual_param_dt"><span class="parameter">name</span></p>
<p class="manual_param_dd">This parameter specifies the name of a previously defined HTML page footer. If a <span class="smallblock">BLANK</span> string or <span class="smallblock">NULL</span> is passed, mPDF will use the value '_default' if such a page footer exists.</p>
<p class="manual_param_dt"><span class="parameter">side</span></p>
<p class="manual_param_dd">Specify whether to set the footer for <span class="smallblock">ODD</span> or <span class="smallblock">EVEN</span> pages in a <span class="smallblock">DOUBLE-SIDED</span> document.

<span class="smallblock">DEFAULT</span>: 'O'</p>
<p class="manual_param_dd"><b>Values</b> (case-sensitive)

O - set the footer for <span class="smallblock">ODD</span> pages in a <span class="smallblock">DOUBLE-SIDED</span> document, or for both <span class="smallblock">ODD</span> and <span class="smallblock">EVEN</span> in a <span class="smallblock">SINGLE-SIDED</span> document.

E - set the footer for <span class="smallblock">EVEN</span> pages

<span class="smallblock">DEFAULT</span> - sets the footer for <span class="smallblock">ODD</span> in a <span class="smallblock">DOUBLE-SIDED</span> document, or for both <span class="smallblock">ODD</span> and <span class="smallblock">EVEN</span> in a <span class="smallblock">SINGLE-SIDED</span> document.</p>
<h2>Changelog</h2>
<table class="bpmTopic"> <thead>
<tr> <th>Version</th><th>Description</th> </tr>
</thead> <tbody>
<tr>
<td>2.0</td>
<td>The function was added.</td>
</tr>
</tbody> </table>
<h2>Examples</h2>
<p>For examples and further information please see:</p>
<ul>
<li class="manual_boxlist"><a href="/headers-footers/headers-footers.html">Headers &amp; Footers</a></li>
<li class="manual_boxlist"><a href="/headers-footers/method-4.html">Headers &amp; Footers - Method 4</a></li>
</ul>
<h2>See Also</h2>
<ul>
<li class="manual_boxlist"><a href="/reference/mpdf-functions/defhtmlfooterbyname.html">DefHTMLFooterByName()</a></li>
<li class="manual_boxlist">&lt;<a href="/reference/html-control-tags/htmlpagefooter.html">htmlpagefooter</a>&gt;</li>
<li class="manual_boxlist"><a href="/reference/mpdf-functions/sethtmlheaderbyname.html">SetHTMLHeaderByName()</a></li>
<li class="manual_boxlist">&lt;<a href="/reference/html-control-tags/sethtmlpagefooter.html">sethtmlpagefooter</a>&gt;</li>
</ul>
<p>&nbsp;</p>
</div>
</div>
