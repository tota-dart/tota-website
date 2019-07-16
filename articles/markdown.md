---
title: 'Markdown'
description: 'Markdown is great'
template: "posts.mustache"
public: true
date: "2019-06-02"
tags:
  - "fun"
---

# Markdown

Markdown is **great**!

* It has lists.
* It has [links](http://example.com).
* And even code blocks:

```dart
Future<String> greet(String name) => Future.value("Hello, $name!");

Future<void> main() async {
  try {
    var msg = await greet('world');
    print(msg);
  catch (e) {
    print(e.message);
  }
}
