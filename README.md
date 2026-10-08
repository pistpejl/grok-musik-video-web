# Grok Musik Video (web)

Static build of the [Grok Musik Video](https://github.com/pistpejl/grok-musik-video) web app.
This repository contains **only** the exported website: no server code and no API keys.

The backend (NVIDIA proxy, ffmpeg, Piper) runs elsewhere. The page reads its address at
startup from `config.js`:

```js
window.GMV_CONFIG = { proxyUrl: "https://your-proxy.example" };
```

When the proxy tunnel URL changes, edit that one line and push to `gh-pages`. No rebuild needed.
You can also override it in the app under Inställningar → Server (webb); that value stays in
your browser only.

Site: https://pistpejl.github.io/grok-musik-video-web/
