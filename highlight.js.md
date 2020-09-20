---
layout: page
title: Highlight.js Themes
permalink: /highlight.js/
---

 <link rel="stylesheet2"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-dark.min.css">
      


<html>
<head>

<link 
  href="http://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.3.0/css/font-awesome.css" 
  rel="stylesheet"  type='text/css'>
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
background: -webkit-linear-gradient(45deg, #FA8BFF 0%, #2BD2FF 52%, #2BFF88 90%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
    border: solid 1px;
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
  background: -webkit-linear-gradient(45deg, #FA8BFF 0%, #2BD2FF 52%, #2BFF88 90%);
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

:root {
   --style:gradient-light
}

[data-theme="dark"] {
--style:gradient-dark
}

<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/var(--style).min.css">


<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

  <pre><code>
#Test 
  </code></pre>
</div>

<script>
const toggleSwitch = document.querySelector('.theme-switch input[type="checkbox"]');

function switchTheme(e) {
    if (e.target.checked) {
        document.documentElement.setAttribute('data-theme', 'dark');
    }
    else {
        document.documentElement.setAttribute('data-theme', 'light');
    }    
}

toggleSwitch.addEventListener('change', switchTheme, false);
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
  <p style='font-size:10px; color:#9c9c9c'>switch theme</p>
</div>
</body>
</html>
