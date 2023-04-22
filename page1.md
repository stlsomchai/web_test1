---
layout: default
title: My website
output:
  html_document:
    toc: FALSE
---

**Welcome to my website!**


# Getting started

Click the links in the menu above to look around.


# Notes

This website is a collection of regular (R)Markdown document, so you can use all the usual formatting.

If you are new to R Markdown, you can learn more about it [on the R Markdown website](https://rmarkdown.rstudio.com/). 

I also have a discussion of R Markdown and reproducibility [on one of my course pages](https://andreashandel.github.io/MADAcourse/1e_ToolsforReproducibility.html). You'll find additional links to potentially useful R Markdown (and Github) resources there.



<h1> {{ page.title }} </h1>

## Liquid lets you do a lot!


{{ page.title | upcase }}

{{ page.title | remove: "and" }}

{{ 'logo' | append: '.jpg' }}

{{ "I wish I was an Oscar Myers weiner." | truncatewords: 4 }}

{% unless page.title == 'Home Page' %}
  This is not the home page.
{% endunless %}

{% if page.title == 'Liquid objects tags and filters' %}
  Jekyll Liquid is so kewl!
{% endif %}


{% assign favorite_food = 'unhealthy' %}

My favorite food is {{ favorite_food }}.

{% assign first_time_visitor = true %}
{% if first_time_visitor == true %}
  Welcome to the site!
{% endif %}
