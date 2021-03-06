---
layout: with-sidebar
sidebar: documentation
custom_js:
- /js/function_listing.js
title: Double Datatype
audience: documentation
type: datatype
versions:
- 2.0
- 2.1
datatype: double
definition:
  type: number
  format: double
---

{% include numeric_types.html %}

Doubles are double-precision numbers.  They can represent any number exactly, except for numbers whose digits repeat infinitely.

Since Doubles can be either larger or more precise than what JSON parsers allow, many formats, such as [JSON](/docs/formats/json.html), serialize them as strings. For example:

{% highlight javascript %}
[ {
  "double_column" : "42"
} ]
{% endhighlight %}


The following table describes the operators that can be used with Doubles. 

| Operation     | Description                                                     |
| ---           | ---                                                             |
| `<`           | `TRUE` for numerics less than this one.                         |
| `<=`          | `TRUE` for numerics that are less than or equal to this one.    |
| `>`           | `TRUE` for numerics that are greater than this one.             |
| `>=`          | `TRUE` for numerics that are greater than or equal to this one. |
| `!=`          | `TRUE` for numerics that are not equal to this one.             |
| `=`           | `TRUE` for numerics that are equal to this one.                 |
| `IS NULL`     | `TRUE` for numerics that are `NULL`.                            |
| `IS NOT NULL` | `TRUE` for numerics that are not `NULL`.                        |
| `+`           | Adds two numerics                                               |
| `-`           | Subtracts one numeric from another                              |
| `*`           | Multiplies two numerics                                         |
| `/`           | Divides one numeric by another                                  |
| `%`           | Returns the modulo of one numeric divided by another            |
| `^`           | Returns the modulo of one numeric divided by another            |

The following table describes the functions that can be used with Doubles.

{% include function_listing.html datatype="double" %}
