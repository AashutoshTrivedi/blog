---
layout: post
title:  "What is Jekyll?"
date:   2020-12-02
comments: true
categories: jekyll update
img: https://jekyllrb.com/img/jekyll-og.png
k: true
---

Jekyll is a static site generator that used liquid template language to convert markdown and html pages to static sites that are ready to be served.
Github has build in support for Jekyll and so it can be really useful to generate and deploy static websites on GitHub as git pages.

One more clarification that I want to make here is that static pages do include any front end technology like JavaScript, react, etc. Only thing is it does not interact with the user and do any dynamic thing which requires sending or receiving data once page is rendered.

Jekyll also offers powerful support for code snippets:

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```
Liquid template for loop

``` bash

{% for i in (1..5) %}
  {% if i == 4 %}
    {% break %}
  {% else %}
    {{ i }}
  {% endif %}
{% endfor %}

```

To find [more](https://shopify.github.io/liquid/tags/iteration/)





Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
