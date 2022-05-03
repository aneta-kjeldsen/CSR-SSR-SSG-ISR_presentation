<img src="./dist/icons/fa-circle-check.svg" class="heading--icon" />

- quick initial access <!-- .element: class="fragment fade-in" -->
- great First Contentful Paint score<!-- .element: class="fragment fade-in" -->
- great for SEO<!-- .element: class="fragment fade-in" -->
- personalisation is much easier<!-- .element: class="fragment fade-in" -->

Note:
- in theory pages are immediately available to interact with, on CSR app, users can’t interact with website until the JS bundle is 100% loaded
- SSR can give a great First Contentful Paint score, which improves the user experience
- search engines don’t need to run JS to read and index content, CSR websites get indexed as well, but not as fast as SSR
- enables teams to provide dynamic content experiences that can be personalised


<img src="./dist/icons/fa-circle-xmark.svg" class="heading--icon" />

- more calls to the server<!-- .element: class="fragment fade-in" -->
- slower than SPAs and SSGs<!-- .element: class="fragment fade-in" -->
- vulnerability<!-- .element: class="fragment fade-in" -->
- complex caching<!-- .element: class="fragment fade-in" -->
- server costs<!-- .element: class="fragment fade-in" -->
- higher latency<!-- .element: class="fragment fade-in" -->

Note: 
- it is important to make sure your infrastructure can handle the requests to the servers and that the servers are able to easily scale as traffic continues to rise
- browsing from page to page - call to server each time, loading everything on demand will give slower UX flow
- SSR sites are harder to keep secure because they have a bigger surface to attack than CSR sites (not only XSS - cross site scripting, but also i.e. SQL injection)
- configuring cache is usually more complex on SSR sites
- SSR often needs a bigger and more powerful server to provide high-performance than CSR
- SSR sites tend to get a high latency (ping rate), so if there is a lot of traffic at the same time, it will slow down the browsing experience for everyone. CSR doesn’t suffer from this nearly as much.