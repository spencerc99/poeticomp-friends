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

For now, you can import the file directly from github:

```html
<script type="module">
  fetch(
    "https://raw.githubusercontent.com/spencerc99/poeticomp-friends/main/webring.json"
  )
    .then((c) => c.json())
    .then((webring) => {
      console.log(webring);
    });
</script>
```

This would be sufficient on its own if we had native support for [importing JSON files](https://github.com/tc39/proposal-import-attributes) which is still in development in the official HTML spec. But for now, they don't support any file type that is not explicitly javascript.
