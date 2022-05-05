<img src="./dist/icons/fa-circle-check.svg" class="heading--icon" />

- quick initial access <!-- .element: class="fragment fade-in" -->
- great First Contentful Paint score<!-- .element: class="fragment fade-in" -->
- great for SEO<!-- .element: class="fragment fade-in" -->
- personalisation is much easier<!-- .element: class="fragment fade-in" -->

Note:
- in theory pages are faster available to interact with
- can give a great First Contentful Paint score, which improves UX
- search engines don’t need to run JS to read and index content
- enables teams to provide dynamic content experiences that can be personalised


<img src="./dist/icons/fa-circle-xmark.svg" class="heading--icon" />

- more calls to the server<!-- .element: class="fragment fade-in" -->
- poorer UX when browsing from page to page<!-- .element: class="fragment fade-in" -->
- vulnerability<!-- .element: class="fragment fade-in" -->
- complex caching<!-- .element: class="fragment fade-in" -->
- server costs<!-- .element: class="fragment fade-in" -->
- higher latency<!-- .element: class="fragment fade-in" -->

Note: 
- infrastructure can handle requests and the servers are able to scale as traffic grows
- call to server each time and loading everything on demand will give slower UX flow
- SSR sites are harder to keep secure because they have a bigger surface to attack than CSR sites
- configuring cache is usually more complex
- SSR often needs a bigger and more powerful server to provide high-performance than CSR
- SSR sites tend to get a high latency (ping rate), so if there is a lot of traffic at the same time, it will slow down the browsing experience for everyone