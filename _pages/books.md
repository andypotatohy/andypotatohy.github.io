---
layout: book-shelf
title: Bookshelf
permalink: /books/
nav: true
nav_order: 4
collection: books
---

> “書中自有黃金屋”
>
> -- Chinese proverb (A book holds a house of gold)

## Books that I am reading, have read, or will read
{% assign book_items = site.books | sort: 'date' | reverse %}

{% for item in book_items %}
  <h3>{{ item.title }}</h3>
  <p>{{ item.content }}</p>
{% endfor %}
