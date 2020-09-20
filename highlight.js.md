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

.btn {
  border-radius: 3px;
  background:transparent;
   border: solid 1px #9c9c9c;
   color: #9c9c9c;
   display: inline-block;
   font-family: "Raleway", Helvetica, sans-serif;
   font-size: .7em !important;
   font-weight: 800;
   height: 1.5em;
   letter-spacing: 0em;
   line-height: 1.5em;
   margin: auto;
   padding: 0 .6em;
   -moz-transition: background-color 0.2s ease, border 0.2s ease, color 0.2s ease;
   -webkit-transition: background-color 0.2s ease, border 0.2s ease, color 0.2s ease;
   -ms-transition: background-color 0.2s ease, border 0.2s ease, color 0.2s ease;
   transition: background-color 0.2s ease, border 0.2s ease, color 0.2s ease;
   text-align: center;
   text-transform: capitalize;
   width: fit-content;
   background-color:transparent;
}

.btn:hover {
    color:#2EBAAE; 
    border: solid 1px #2EBAAE;
}

.theme-switch-wrapper {
  display: inline-block;
  padding-top: 0px;
  padding-left:25em;
  align-items: center;

  em {
    margin-left: 10px;
    font-size: 10px;
  }
}
.theme-switch {
  display: inline-block;
  height: 34px;
  position: relative;
  width: 60px;
}

.theme-switch input {
  display:none;
}

.slider {
  background-color: #ccc;
  bottom: 0;
  cursor: pointer;
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
  transition: .4s;
}

.slider:before {
  background-color: #fff;
  bottom: 4px;
  content: "";
  height: 26px;
  left: 4px;
  position: absolute;
  transition: .4s;
  width: 26px;
}

input:checked + .slider {
  background-color: #66bb6a;
}

input:checked + .slider:before {
  transform: translateX(26px);
}

.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
.myDiv {
  padding: 1em;
  background: #9c9c9c;
  width: 30em;
  border: 1 px solid #3D3D3E;
  
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
#Test 
  </code></pre>
</div>

<script>
function switchTheme(e) {
    if (e.target.checked) {
        document.documentElement.setAttribute('data-theme', 'dark');
        localStorage.setItem('theme', 'dark'); //add this
    }
    else {
        document.documentElement.setAttribute('data-theme', 'light');
        localStorage.setItem('theme', 'light'); //add this
    }    
}
</script>

<div>
  <button class="btn">Python<i class="fab fa-python"></i></button>
  <button class="btn">R<i class="fab fa-r-project"></i></button>
  <button class="btn">JavaScript<i class="fab fa-js-square"></i></button>
  <button class="btn">HTML<i class="fas fa-code"></i></button>
  <button class="btn">CSS<i class="far fa-file-code"></i></button>
</div>

<div class="theme-switch-wrapper">
    <label class="theme-switch" for="checkbox">
        <input type="checkbox" id="checkbox" />
        <div class="slider round"></div>
  </label>
  <em>Switch theme</em>
</div>
</body>
</html>
