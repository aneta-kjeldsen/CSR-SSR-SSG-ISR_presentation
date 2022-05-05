<img src="./dist/icons/fa-circle-check.svg" class="heading--icon" />

- the best from both worlds <!-- .element: class="fragment fade-in" -->
- quick initial access <!-- .element: class="fragment fade-in" -->
- great First Contentful Paint score<!-- .element: class="fragment fade-in" -->
- great UX when browsing from page to page<!-- .element: class="fragment fade-in" -->
- great for SEO<!-- .element: class="fragment fade-in" -->

Note:
- combines the best from both worlds: SSG & SSR
- in theory pages are immediately available to interact with
- can give a great First Contentful Paint score, which improves the UX
- no calls to server each time when users navigates on the page
- search engines don’t need to run JS to read and index content


<img src="./dist/icons/fa-circle-xmark.svg" class="heading--icon" />

- not most up-to-date version <!-- .element: class="fragment fade-in" -->
- inconsistent experience <!-- .element: class="fragment fade-in" -->
- no atomic and immutable deployment <!-- .element: class="fragment fade-in" -->
- debugging is difficult <!-- .element: class="fragment fade-in" -->

Note: 
- when user comes to page, you want them to see the most up-to-date version immediately, that's not the case
- can have negative side-effects on UX as a result of old/unbuilt pages
- rollbacks can no longer be instant, and you no longer have that single new version of your site when you update your content
- different users (and the dev team!) would see different pages, and it might be difficult to duplicate