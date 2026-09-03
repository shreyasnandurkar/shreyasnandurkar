<p align="center">
  <img src="./assets/banner.svg" width="100%" alt="Shreyas Nandurkar — Backend Engineer" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/shreyas-nandurkar"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>&nbsp;
  <a href="mailto:shreyasn1105@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>&nbsp;
  <a href="https://github.com/shreyasnandurkar"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" /></a>&nbsp;
  <a href="https://codeforces.com/profile/lithium2006"><img src="https://img.shields.io/badge/Codeforces-Expert-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" /></a>&nbsp;
  <a href="https://leetcode.com/u/lithium2006"><img src="https://img.shields.io/badge/LeetCode-2142-FFA116?style=flat-square&logo=leetcode&logoColor=white" /></a>
</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:6366F1,50:8B5CF6,100:22D3EE&height=3" />

## About

Final-year Computer Science student at Manipal Institute of Technology, Bengaluru, focused on backend engineering with Java and Spring Boot. I build production systems end to end — a live URL-shortener product, an OpenAI-compatible LLM gateway, and a real-time image-streaming application — with an emphasis on clean architecture, concurrency, and performance. Co-founder and founding engineer at GoLinkGone.

## Featured Projects

### &nbsp;🔗&nbsp; GoLinkGone &nbsp;·&nbsp; <sub>live URL shortener & link-management platform</sub>

Co-founder and backend engineer. Short links, click analytics, and customizable QR code studio, serving real users. **27K+ pageviews in just ~1.5 Months · 500+ Sign-Ups · 550+ short links created · 22k+ redirects served.** Ranked #9 of 100+ products on Peerlist (Week 26); also launched on Product Hunt.

- **Customizable QR codes** — branded QR generation driven by a validated JSONB style configuration, persisted in custom storage and re-rendered on demand.
- **Analytics pipeline** — a 10K-capacity click queue drained every 3 seconds via map/reduce into batched upserts, with murmur3-hashed visitor IDs on a virtual-thread executor.
- **Platform** — Caffeine caching, ES256 JWT auth, Bucket4j rate limiting, MaxMind GeoLite2 geolocation, host-based dual-domain routing, Supabase auth with Google SSO.

<p>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
</p>

<a href="https://golinkgone.com"><img src="https://img.shields.io/badge/Live-8B5CF6?style=flat-square&logo=googlechrome&logoColor=white" /></a>&nbsp;
<a href="https://github.com/go-link-gone/glg-backend"><img src="https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white" /></a>

### &nbsp;♟️&nbsp; BotvinnikAPI &nbsp;·&nbsp; <sub>OpenAI-compatible LLM gateway</sub>

A single endpoint that routes, load-balances, and fails over across multiple LLM providers (Ollama, Gemini) while presenting the OpenAI wire protocol to clients, so standard SDKs and tools work unmodified.

- **Reactive core** — Spring WebFlux with R2DBC; SSE streaming with cross-provider chunk normalization.
- **Routing & resilience** — power-of-two-choices load balancing on live in-flight depth, TTFT-based provider health states, circuit breakers with connect-time failover.
- **Security** — SHA-256 gateway keys, AES-GCM-256 provider credentials, connect-time SSRF guard, per-key rate limits and spend caps.
- **Verified** — ~0.3 ms p50 gateway overhead, zero errors at 200 concurrent, 93 tests including failure injection.

<p>
  <img src="https://img.shields.io/badge/Java_25-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot_4.1-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/WebFlux-6DB33F?style=flat-square&logo=spring&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL_·_R2DBC-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

<a href="https://github.com/shreyasnandurkar/botvinnik-api"><img src="https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white" /></a>

### &nbsp;🎇&nbsp; Pixel Mosaic &nbsp;·&nbsp; <sub>real-time image reconstruction in the browser</sub>

Rebuilds the subject of one image using the pixels of another, streamed to a WebGL client and played back as an animated particle system.

- **AI subject extraction** — U²-Net saliency model served via ONNX Runtime.
- **Streaming** — custom binary WebSocket protocol (32-byte header + 256 KB chunks) feeding a Three.js instanced-points renderer with custom shaders.
- **Concurrency** — dual-lane processing pipeline with buffer pooling, a global concurrency semaphore, and per-IP rate limiting.
- Tried and loved by **100+** people.

<p>
  <img src="https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot_3.2-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

<a href="https://shreyasnandurkar.github.io/pixel-mosaic/"><img src="https://img.shields.io/badge/Live_Demo-8B5CF6?style=flat-square&logo=googlechrome&logoColor=white" /></a>&nbsp;
<a href="https://github.com/shreyasnandurkar/pixel-mosaic"><img src="https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white" /></a>

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:6366F1,50:8B5CF6,100:22D3EE&height=3" />

## Tech Stack

**Languages**

<img src="https://skillicons.dev/icons?i=java,python,c,cpp,js,ts&theme=dark" height="44" />

**Backend**

<img src="https://skillicons.dev/icons?i=spring,hibernate,kafka&theme=dark" height="44" />

**Data**

<img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis&theme=dark" height="44" />

**Infrastructure & Tools**

<img src="https://skillicons.dev/icons?i=docker,git,maven,postman,idea&theme=dark" height="44" />

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:6366F1,50:8B5CF6,100:22D3EE&height=3" />

## Competitive Programming

Codeforces Expert · LeetCode Guardian (2142) · active on CodeChef and AtCoder.

- **1st place** — MAHE CodeWars 2026 &nbsp;(3rd place, 2025)
- **Top 5 Finalist** — Hitachi Visisonics AI'26
- Preparing for ICPC regionals

<a href="https://codeforces.com/profile/lithium2006"><img src="https://img.shields.io/badge/Codeforces-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" /></a>&nbsp;
<a href="https://leetcode.com/u/lithium2006"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white" /></a>&nbsp;
<a href="https://www.codechef.com/users/venus2006"><img src="https://img.shields.io/badge/CodeChef-5B4638?style=flat-square&logo=codechef&logoColor=white" /></a>&nbsp;
<a href="https://atcoder.jp/users/venus2006"><img src="https://img.shields.io/badge/AtCoder-222222?style=flat-square&logo=atcoder&logoColor=white" /></a>&nbsp;
<a href="https://geeksforgeeks.org/user/shreyaswmsg/profile"><img src="https://img.shields.io/badge/GeeksforGeeks-2F8D46?style=flat-square&logo=geeksforgeeks&logoColor=white" /></a>

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:6366F1,50:8B5CF6,100:22D3EE&height=3" />

## GitHub Stats

<p align="center">
  <img height="165" src="https://github-stats-extended.vercel.app/api?username=shreyasnandurkar&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&title_color=8B5CF6&icon_color=22D3EE&text_color=94A3B8&bg_color=0B1021&hide_rank=true" />
  <img height="165" src="https://github-stats-extended.vercel.app/api/top-langs?username=shreyasnandurkar&layout=compact&hide_border=true&hide=html,css,scss&langs_count=8&title_color=8B5CF6&text_color=94A3B8&bg_color=0B1021" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=shreyasnandurkar&hide_border=true&background=0B1021&ring=8B5CF6&fire=22D3EE&currStreakLabel=8B5CF6&sideLabels=94A3B8&dates=64748B&currStreakNum=F1F5F9&sideNums=F1F5F9&stroke=8B5CF6" />
</p>
