```js [6|7|14-16|10-13|22-24]
import { useEffect, useState } from "react";
import Todo from "@components/Todo";
import Loading from "@components/Loading";
import { getTodos } from "./api";

export default function ClientSideRendered() {
  const [data, setData] = useState([]);
  const [isLoading, setIsLoading] = useState(true);

  async function getData() {
    setData(await getTodos());
    setIsLoading(false);
  }
  useEffect(() => {
    getData();
  }, []);
  return (
    <main>
      <h1>CSR - Client Side Render</h1>
      <h3>My TODO list:</h3>
      {isLoading && <Loading></Loading>}
      {data.map((item) => (
        <Todo key={item.id} item={item}></Todo>
      ))}
    </main>
  );
}
```


```html [1-3|4]
<script defer="" nomodule="" src="/_next/static/chunks/polyfills-5cd94c89d3acac5f.js"></script>
...
<script src="/_next/static/9lWyBGzmGgJ1QhbbI6MP-/_middlewareManifest.js" defer=""></script>
<div id="__next" data-reactroot=""></div>
```