<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/harisvreto/harisvreto/main/signature-dark.png">
  <img src="https://raw.githubusercontent.com/harisvreto/harisvreto/main/signature-light.png" alt="Haris Vreto" width="295">
</picture>

### `hv_` — I make products people love.

**[harisvreto.dev](https://harisvreto.dev)** · [LinkedIn](https://www.linkedin.com/in/harisvreto/) · [CV (PDF)](https://harisvreto.dev/cv.pdf) · [/llms.txt](https://harisvreto.dev/llms.txt)

</div>

---

## `$ whoami`

Hi, I'm **Haris** 👋 — a senior full-stack engineer at [Inkitt](https://www.inkitt.com) (San Francisco), shipping from Sarajevo. Ten-plus years across publishing, Web3 and healthcare; hobby UI/UX designer; AI running through every stage of my workflow — agentic coding, AI-assisted review, generated tests. The gap between *idea* and *shipped* has never been smaller, and I intend to keep abusing that.

```text
BUILDING    Inkitt platform · Penna · HV-1 (my portfolio's zero-API chatbot)
BASED       Sarajevo · GMT+1, SF hours
RUNNING ON  Bosnian coffee, unreasonable amounts
OPEN TO     interesting problems
```

That signature above isn't an image of my signature. It's drawing itself, right now, from about a kilobyte of path data — see below.

## `$ cat penna.md`

**[Penna](https://penna.harisvreto.dev)** — draw a signature, watch it write itself back, then take it away as an SVG that animates on its own. No JavaScript in the file. **1.3 KB.**

Every stroke becomes one `<path>` with a `stroke-dasharray` equal to its own arc length, and one generated `@keyframes` rule walks `stroke-dashoffset` to zero during that stroke's slice of a shared timeline. There's no runtime, because CSS *is* the runtime. Stroke duration comes from arc length rather than a fixed number, which is the whole difference between reading as handwriting and reading as playback.

The same signature as an animated GIF is 228 KB — **175× bigger**, and it looks worse.

The mark in my portfolio's header is a Penna export. So is the one at the top of this README, which had to be APNG instead of SVG: GitHub proxies images and strips the `<style>` block, so a self-animating SVG arrives frozen. That one rendering quirk is the entire reason the APNG exporter exists.

Vite · React · TypeScript, with the geometry/timeline/SVG engine kept dependency-free. 40 tests, Lighthouse **100 across all four** categories.

## `$ cat portfolio.md`

**[harisvreto.dev](https://harisvreto.dev)** is a narrow single column: a short intro, [projects](https://harisvreto.dev/projects), and [writing](https://harisvreto.dev/writing). Its centerpiece is **HV-1**, a chatbot with **zero API calls** — the "model" is a hand-written TypeScript intent matcher trained on exactly one career (mine). It streams answers, renders project cards and timelines inline, survives offline, and costs nothing to run. Sometimes the right model is no model.

The punchline: a real AI helped build the fake one — the whole site was developed agentically with Claude Code, then reviewed like any PR.

**Worth poking at over there:**

- 🟩 Terminal easter eggs — press <kbd>⌘K</kbd> and try `sudo hire haris`, `rm -rf /`, or "roast his tech stack"
- ✍️ A header wordmark that writes itself on load, pure CSS on server-rendered markup — no hydration gate, no JS
- 📝 [Essays](https://harisvreto.dev/writing) on why the right model is often no model, why boring releases are a feature, and how a signature ends up smaller than a favicon
- 📄 An ATS-friendly CV generated at build time from the same data that powers the page, the chat and [`/llms.txt`](https://harisvreto.dev/llms.txt) — nothing can drift
- 💯 Lighthouse 100 on SEO · a11y · best practices, CLS 0, zero third-party requests, no cookies

**Stack these days:** TypeScript · React · Next.js · React Native · Node.js · NestJS · Rails · GraphQL · AWS — with Claude Code, Cursor and the Vercel AI SDK as the leverage layer.

## `$ ping haris`

Fastest: **[harisvreto.astra@gmail.com](mailto:harisvreto.astra@gmail.com)** — or ask [the terminal](https://harisvreto.dev) anything first; it knows my decade of shipping cold.

<div align="center">

`$ status: ● all systems shipping — open to interesting problems`

</div>
