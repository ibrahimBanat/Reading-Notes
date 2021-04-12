# EJS Partials

Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.

- `EJS Partials` help us avoid repetition of the same code on several web pages.

- EJS partials work like EJS layouts too in creating a single fix content on a web page.

Partials come in handy when you want to reuse the same HTML across multiple views.

creating and including partials is very straightforward with EJS.

```
<%- include('partials/footer') %>
```
