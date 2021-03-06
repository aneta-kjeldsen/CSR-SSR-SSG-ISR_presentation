```js  [18|19|22-27|5|11-13]
import Todo from "@components/Todo";
import Loading from "@components/Loading";
import { getTodos } from "./api";

export default function ServerSideRendered({ data, isLoading = true }) {
  return (
    <main>
      <h1>SSR - Server Side Render</h1>
      <h3>My TODO list:</h3>
      {isLoading && <Loading><Loading />}
      {data.map((item) => (
        <Todo key={item.id} item={item}></Todo>
      ))}
    </main>
  );
}

export async function getServerSideProps() {
  const data = await getTodos();
  const isLoading = false;

  return {
    props: {
      data,
      isLoading,
    },
  };
}
```


```html [1-3|4-11]
<script defer="" nomodule="" src="/_next/static/chunks/polyfills-5cd94c89d3acac5f.js"></script>
...
<script src="/_next/static/9lWyBGzmGgJ1QhbbI6MP-/_middlewareManifest.js" defer=""></script>
<div id="__next" data-reactroot="">
    <p>1 - 🌮 Make Homemade Natto</p>
    <p>2 - 🏝 Explore the Galapagos Islands</p>
    <p>3 - 🎞 Go to a Big Time Movie Premiere in Hollywood</p>
    <p>4 - 💃 Look Drop Dead Gorgeous</p>
    <p>5 - 🍹 Taste Mojito</p>
    <p>6 - 📸 Take a Picture With an Interesting Stranger</p>
</div>
```