---
layout: post
permalink: setup
---


<!-- header.html -->
<!-- 
  <a href="{{ site.baseurl }}/" class="header_logo">
    <svg viewBox="39.8 505.2 171.7 195">
      <title>Sam Pedley Logo</title>
      <g>
        <path class="sLogoMain" d="M55.5 680.4L39.8 505.2h171.7L196 680.4l-70.5 19.8" fill="#4583B3"/>
        <path class="sLogoSecondary" d="M125.9 685l56.7-15.6 13.4-150h-70.1" fill="#79A7CB"/>
        <g>
          <polygon points="125.5 584.5 125.5 606.1 152.2 606.1 149.5 633.9 125.5 640.4 125.5 662.9 169.6 650.7 170.1 646.9 175 590.2 175.7 584.5 169.6 584.5 " fill="#FFF"/>
          <polygon points="125.3 550.2 125.7 550.2 149.6 556.7 151.2 573.8 162.6 573.8 172.5 573.8 169.8 539.9 125.7 527.7 125.3 527.7 " fill="#FFF"/>
        </g>
          <polygon points="125.7 606.1 125.7 584.5 99 584.5 101.7 556.7 125.7 550.2 125.7 527.7 81.5 539.9 81.1 543.7 76.1 600.4 75.4 606.1 81.5 606.1 " fill="#EBEBEB"/>
          <polyline class="sLogoMain" points="69.7 602.4 60.7 593.2 71.7 582.5 100.6 612.3 89.6 622.9 " fill="#4583B3"/>
          <polygon class="sLogoSecondary" points="180.2 606.7 151.1 577.3 175.4 580 177.8 582.3 " fill="#79A7CB"/>
          <polygon points="125.9 640.4 125.5 640.4 101.5 633.9 99.9 616.8 88.5 616.8 78.7 616.8 81.3 650.7 125.5 662.9 125.9 662.9 " fill="#EBEBEB"/></g>
        </svg>
  </a>
-->

<!-- head.html -->

<!-- <meta name="twitter:card" content="summary" /> -->
<!-- <meta name="twitter:site" content="@sam_pedley" /> -->
<!-- <meta name="twitter:creator" content="@sam_pedley" /> -->



To Do LIst

1. hackcss

把hackcss的grid、button的样式合并到里面。

2. img图床

config 设置一个 imgurl

3. 



# Docs

## Configuration

This theme can be configured by modifying the `_config.yml` file.

### Theme settings

This theme supports three different mode provided by `hack.css`:

- `standard`
- `markdown`
- `dark`

Set `theme_mode` to the desired value.

### Available customizations

- `your_name` and `email` strings to display them in different places on site
- `navigation` is an array of `text` and `url` pairs to render the menu
- `projects` is a setting that contains data for the `examples` page, every item must contain `name` and `link`, `image` and `description` are optional
- `social` contains an array of three required params: `service` is used to include a service icon by the {% raw %}`{% include icon-{{ service }}.html %}`{% endraw %} command, `username` and `link` are quite obvious



<fieldset class="form-group form-success">
  <label for="phone">Phone Number:</label>
  <input id="phone" type="text" placeholder="" class="form-control">
  <div class="help-block">In this format: +86 xxx xxx xxxxx</div>
</fieldset>



<!-- with only an arrow -->
<div class="progress-bar">
  <div class="progress-bar-filled" style="width: 40%"></div>
</div>

<!-- with a percentage showing above the arrow -->
<div class="progress-bar progress-bar-show-percent">
  <div class="progress-bar-filled" style="width: 40%" data-filled="Loading 40%"></div>
</div>



<button class="btn btn-default">Default</button>
<button class="btn btn-primary">Primary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-info">Info</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-error">Error</button>

<button class="btn btn-primary btn-ghost">Ghost Button</button>

<button class="btn btn-primary btn-block">Block Level Button</button>


<div class="card">
  <header class="card-header">title</header>
  <div class="card-content">
    <div class="inner">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Expedita, quas ex vero enim in doloribus officiis ullam vel nam esse sapiente velit incidunt. Eaque quod et, aut maiores excepturi sint.</div>
  </div>
</div>



<div class="alert alert-success">Success message</div>
<div class="alert alert-info">Info message</div>
<div class="alert alert-warning">Warning message</div>
<div class="alert alert-error">Error message</div>


<div class="loading"></div>
