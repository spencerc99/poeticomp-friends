# poeticomp-friends

the poeticomp friends webring and associated gadgets.

- [ ] make the webring importable as a javascript object so you can do (also enables npm import to use in react / JS framework projects):

```html
<script type="module">
  import { webring } from "https://unpkg.com/poeticomp-friends";
  for (const friend of webring) {
    document.body.appendChild(friend);
  }
</script>
```
