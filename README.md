## Up and running

**Env Dependencies:**
* [Ruby](https://www.ruby-lang.org/en/downloads/)
* [Sass](http://sass-lang.com/)
* [jekyll](https://rubygems.org/gems/jekyll/)
* [bundler](https://rubygems.org/gems/bundler)

**Helpful Commands:**
* `bundle exec jekyll serve` for local dev on port `4000`.
    * Or `npm run dev` cuz reasons.
* `jekyll build` for not dev.
    * Or `npm run build` cuz other reasons.


 # border: 1px solid $color-riverBed;
 # margin: 0.75rem (-$horzPad);

 ## Jekyll theme

 * [theme](https://github.com/SamPedley)


include/head.html

{% if page.title %}
  {% assign title = page.title %}
{% else %}
  {% assign title = site.title %}
{% endif %}