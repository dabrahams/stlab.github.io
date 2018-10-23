---
layout: function
title: operator!=
owner: sparent
brief: Inequality operator
tags:
  - function
defined-in-file: stlab/copy_on_write.hpp
overloads:
  _Bool operator!=(const copy_on_write<T> &, const copy_on_write<T> &):
    annotation:
      - public
    arguments:
      - description: __OPTIONAL__
        name: x
        type: const copy_on_write<T> &
      - description: __OPTIONAL__
        name: y
        type: const copy_on_write<T> &
    description: Operator against same `copy_on_write` type
    return: __OPTIONAL__
    signature_with_names: _Bool operator!=(const copy_on_write<T> & x, const copy_on_write<T> & y)
  _Bool operator!=(const copy_on_write<T> &, const stlab::copy_on_write::element_type &):
    annotation:
      - public
    arguments:
      - description: __OPTIONAL__
        name: x
        type: const copy_on_write<T> &
      - description: __OPTIONAL__
        name: y
        type: const stlab::copy_on_write::element_type &
    description: Operator against `element_type` as rhs
    return: __OPTIONAL__
    signature_with_names: _Bool operator!=(const copy_on_write<T> & x, const stlab::copy_on_write::element_type & y)
  _Bool operator!=(const stlab::copy_on_write::element_type &, const copy_on_write<T> &):
    annotation:
      - public
    arguments:
      - description: __OPTIONAL__
        name: x
        type: const stlab::copy_on_write::element_type &
      - description: __OPTIONAL__
        name: y
        type: const copy_on_write<T> &
    description: Operator against `element_type` as lhs
    return: __OPTIONAL__
    signature_with_names: _Bool operator!=(const stlab::copy_on_write::element_type & x, const copy_on_write<T> & y)
---