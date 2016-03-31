---
layout: page
title: Watermarks
parent_title: What Else Can I Do
permalink: /what-else-can-i-do/watermarks.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>You can add a watermark to the page(s) either text (e.g. DRAFT) and/or a background image.</p>
<p>Set the following before writing the HTML code. NB The watermark is added when writing the footer at the end of a page, so it can be set anytime before ending the page/document.</p>
<p>$mpdf-&gt;SetWatermarkText('DRAFT'); // Will cope with UTF-8 encoded text</p>
<p>$mpdf-&gt;watermark_font = 'DejaVuSansCondensed';&nbsp;// Uses default font if left blank</p>
<p>You can alter the transparency values (default = 0.2) using</p>

{% highlight php %}
<?php

$mpdf->watermarkTextAlpha = 0.1;

$mpdf->watermarkImageAlpha = 0.5;
{% endhighlight %}

<p>A watermark image is set by default to print on top of the page contents. The opacity setting will alter the appearance of the text behind the image. You can optionally set the watermark to appear behind the page contents using <span class="parameter">watermarkImgBehind</span>, but note that the image will be hidden by any background colour specified, including table cells and the page background.</p>

<div class="alert alert-info" role="alert"><b>Note:</b> In version 4.4 <span class="parameter">watermarkImgBehind</span> was unintentionally set to <span class="smallblock">TRUE</span> in the <span class="filename">config.php</span> file</div>
<p>Set the watermark(s) to show using: <a href="/reference/mpdf-variables/showwatermarktext.html">showWatermarkText</a> or <a href="/reference/mpdf-variables/showwatermarktext.html">showWatermarkImage</a></p>

<div class="alert alert-info" role="alert"><b>Note:</b> From mPDF &gt;=3.0 you can alternatively use the CSS style for background-image on the &lt;body&gt; tag to create a sort of watermark, although this does not support opacity. The difference is that text, tables etc are written over the top of a background-image; a watermark is actually printed over the top of everything else, but is semi-transparent.</div>
<h2>See</h2>
<ul>
<li class="manual_boxlist"><a href="/reference/mpdf-functions/setwatermarktext.html">SetWatermarkText()</a> - Set the text to use as a Watermark</li>
<li class="manual_boxlist">&lt;<a href="/reference/html-control-tags/watermarktext.html">watermarktext</a>&gt; - HTML equivalent to SetWatermarkText()</li>
<li class="manual_boxlist"><a href="/reference/mpdf-functions/setwatermarkimage.html">SetWatermarkImage()</a> - Set the image to use as a Watermark</li>
<li class="manual_boxlist">&lt;<a href="/reference/html-control-tags/watermarkimage.html">watermarkimage</a>&gt; - HTML equivalent to SetWatermarkImage()</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/watermarkimagealpha.html">watermarkImageAlpha</a> - Specifies the transparency (alpha value) for the watermark image</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/watermarktextalpha.html">watermarkTextAlpha</a> - Specifies the transparency (alpha value) for the watermark text</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/showwatermarktext.html">showWatermarkText</a> - Specifies whether or not to show/print the watermark text

</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/showwatermarktext.html">showWatermarkImage</a> - Specifies whether or not to show/print the watermark image</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/watermark-font.html">watermark_font</a> - Specifies the font to use for Watermark text</li>
<li class="manual_boxlist"><a href="/reference/mpdf-variables/watermarkimgbehind.html">watermarkImgBehind</a> - Specify whether to show the watermark image behind the page contents</li>
</ul>
<p>&nbsp;</p>
</div>
</div>
