---
layout: page
title: Highlight.js Themes
permalink: /highlight.js/
---

 
<html>
<head>
<script src="https://kit.fontawesome.com/5c0609df7f.js" crossorigin="anonymous"></script>
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
  background-color: #9c9c9c;
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

<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-light.min.css" id="js_css">


<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>


  <pre><code id="code">
# Select language to preview highlighting 
  </code></pre>
</div>


<div>
  <button class="btn">Python<i class="fab fa-python"></i></button>
  <button class="btn">R <i class="fab fa-r-project"></i></button>
  <button class="btn">JavaScript <i class="fab fa-js-square"></i></button>
  <button class="btn">HTML <i class="fas fa-code"></i></button>
  <button class="btn">CSS <i class="far fa-file-code"></i></button>
</div>

<div class="theme-switch-wrapper">
    <label class="theme-switch" for="checkbox">
        <input type="checkbox" id="checkbox" />
        <div class="slider round"></div>
  </label>
  <p id="switch_label" style='font-size:10px; color:#9c9c9c'>gradient light</p>
  
  <script>
const toggleSwitch = document.querySelector('.theme-switch input[type="checkbox"]');

function switchTheme(e) {
    if (e.target.checked) {
        document.getElementById("js_css").setAttribute("href", "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-dark.min.css");
        document.getElementById("switch_label").innerHTML = "gradient dark";
    }
    else {
        document.getElementById("js_css").setAttribute("href", "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.2.0/styles/gradient-light.min.css");
        document.getElementById("switch_label").innerHTML = "gradient light";
    }    
}

toggleSwitch.addEventListener('change', switchTheme, false);
</script>

</div>
</body>
</html>
