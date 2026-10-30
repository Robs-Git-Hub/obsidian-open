# obsidian-open

A one-page forwarder that turns an ordinary web link into an `obsidian://` link, so notes can be opened from apps on Android that only accept `https://` links (chat apps, the Claude app).

Link format:

```
https://robs-git-hub.github.io/obsidian-open/#vault=<vault name>&file=<path in vault, no .md>
```

Everything after `#` stays in the browser and is never sent to GitHub, so vault and note names are not logged. The page has no analytics and loads nothing from elsewhere. On Android it uses an `intent://` link for Chrome; elsewhere a plain `obsidian://` link. If the app doesn't open by itself, tap the button.
