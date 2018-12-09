---
layout: default
permalink: setup
---

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



</p>