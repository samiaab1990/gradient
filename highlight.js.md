---
layout: page
title: Highlight.js Themes
permalink: /highlight.js/
---
<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-light.min.css">
      
 <link rel="stylesheet2"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-dark.min.css">
      


<html>
<head>
<style>
.myDiv {
  border: 5px solid #3D3D3E;
  width: 70%;
  height: 70%
  
}
</style>
</head>
<body>

<div class="myDiv">
<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-light.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
  <pre><code>
  function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }

  return (
    <div>
      <web-component>{block}</web-component>
    </div>
  )
}

export  $initHighlight;
  </code></pre>
</div>

</body>
</html>
