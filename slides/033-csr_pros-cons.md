<img src="./dist/icons/fa-circle-check.svg" class="heading--icon" />

- no additional loading required<!-- .element: class="fragment fade-in" -->
- seamless UX<!-- .element: class="fragment fade-in" -->
- code splitting & loading of some parts of UI<!-- .element: class="fragment fade-in" -->
- can be used along with other technologies<!-- .element: class="fragment fade-in" -->

Note:
- while the initial load maybe longer, once the app is fully loaded, no additional loading required
- quick, seamless user experience
- code splitting enables the loading of some parts of UI on demand
- you can use any backend server, put your page on CDN


<img src="./dist/icons/fa-circle-xmark.svg" class="heading--icon" />

- size and complexity<!-- .element: class="fragment fade-in" -->
- SEO<!-- .element: class="fragment fade-in" -->
- difficult to maintain and organise<!-- .element: class="fragment fade-in" -->
- initial load time<!-- .element: class="fragment fade-in" -->

Note:
- as the application grows in size and complexity, it can impact the initial load
- maintaining good SEO is hard - search engines need to run JS to read and index content (websites get indexed as well, but not as fast as SSR)
- large code base for complex web apps can become difficult to maintain and organise
- users can’t interact with website until the JS bundle is 100% loaded