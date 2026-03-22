# Vercel Snippets for Sublime Text

[![Package Control](https://img.shields.io/packagecontrol/dt/Vercel.svg?style=flat-square)](https://packagecontrol.io/packages/Vercel)
[![Sublime Text](https://img.shields.io/badge/Sublime%20Text-3%2F4-ff9800.svg?style=flat-square&logo=sublimetext&logoColor=white)](https://www.sublimetext.com/)
[![License](https://img.shields.io/github/license/renzojohnson/Vercel.svg?style=flat-square)](LICENSE)

140 curated snippets for Vercel development — vercel.json, CLI, Functions, Next.js, AI SDK, Storage, and Deployment.

**Author:** [Renzo Johnson](https://renzojohnson.com)

> This is an unofficial community package and is not affiliated with Vercel Inc.

## Installation

### Package Control (recommended)

1. Open Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
2. Type **Install Package**
3. Search for **Vercel**

### Manual

Clone into your Sublime Text `Packages` directory:

```bash
# macOS
cd ~/Library/Application\ Support/Sublime\ Text/Packages
git clone https://github.com/renzojohnson/Vercel.git

# Linux
cd ~/.config/sublime-text/Packages
git clone https://github.com/renzojohnson/Vercel.git

# Windows
cd %APPDATA%\Sublime Text\Packages
git clone https://github.com/renzojohnson/Vercel.git
```

## Usage

Type `vc:` and browse the autocomplete menu, then press **Tab** to expand.

| Prefix | Category | Count |
|--------|----------|-------|
| `vc:json:` | vercel.json config | 28 |
| `vc:cli:` | CLI commands | 22 |
| `vc:fn:` | Serverless & Edge functions | 20 |
| `vc:next:` | Next.js + Vercel patterns | 30 |
| `vc:env:` | Environment & config | 10 |
| `vc:store:` | Storage (Redis, Postgres, Blob) | 10 |
| `vc:ai:` | AI SDK | 5 |
| `vc:deploy:` | Deployment & CI | 15 |

## Snippet Reference

### vercel.json Config (`vc:json:*`) — 28 snippets

| Trigger | Description |
|---------|-------------|
| `vc:json:init` | vercel.json — minimal starter |
| `vc:json:full` | vercel.json — full config scaffold |
| `vc:json:rewrite` | Rewrite rule |
| `vc:json:rewrites` | Rewrites array with multiple rules |
| `vc:json:redirect` | Redirect rule (301) |
| `vc:json:redirect:permanent` | Permanent redirect (308) |
| `vc:json:redirects` | Redirects array |
| `vc:json:header` | Custom header rule |
| `vc:json:headers` | Headers array with CORS |
| `vc:json:headers:security` | Security headers (CSP, HSTS, X-Frame) |
| `vc:json:cron` | Cron job |
| `vc:json:crons` | Crons array |
| `vc:json:env` | Environment variable |
| `vc:json:functions` | Functions config (memory, maxDuration) |
| `vc:json:functions:region` | Functions with region override |
| `vc:json:regions` | Regions array |
| `vc:json:images` | Images optimization config |
| `vc:json:images:remote` | Remote image patterns |
| `vc:json:framework` | Framework preset |
| `vc:json:build` | Build command override |
| `vc:json:output` | Output directory override |
| `vc:json:install` | Install command override |
| `vc:json:ignore` | Ignored build step command |
| `vc:json:clean` | Clean URLs (trailingSlash, cleanUrls) |
| `vc:json:wildcard` | Wildcard/catch-all rewrite |
| `vc:json:spa` | SPA fallback rewrite |
| `vc:json:api` | API route rewrite |
| `vc:json:github` | GitHub integration config |

### CLI Commands (`vc:cli:*`) — 22 snippets

| Trigger | Description |
|---------|-------------|
| `vc:cli:deploy` | Deploy to preview |
| `vc:cli:deploy:prod` | Deploy to production |
| `vc:cli:deploy:prebuilt` | Deploy prebuilt output |
| `vc:cli:dev` | Start local dev server |
| `vc:cli:env:add` | Add environment variable |
| `vc:cli:env:pull` | Pull env vars to .env.local |
| `vc:cli:env:ls` | List environment variables |
| `vc:cli:env:rm` | Remove environment variable |
| `vc:cli:domains:add` | Add custom domain |
| `vc:cli:domains:ls` | List domains |
| `vc:cli:dns:add` | Add DNS record |
| `vc:cli:logs` | Tail runtime logs |
| `vc:cli:inspect` | Inspect deployment |
| `vc:cli:promote` | Promote deployment to production |
| `vc:cli:rollback` | Rollback to previous deployment |
| `vc:cli:bisect` | Bisect deployments |
| `vc:cli:link` | Link local directory to project |
| `vc:cli:pull` | Pull project settings |
| `vc:cli:build` | Build project locally |
| `vc:cli:project:ls` | List projects |
| `vc:cli:whoami` | Show current user/team |
| `vc:cli:certs` | List SSL certificates |

### Serverless & Edge Functions (`vc:fn:*`) — 20 snippets

| Trigger | Description |
|---------|-------------|
| `vc:fn:node` | Node.js serverless function (@vercel/node) |
| `vc:fn:node:web` | Node.js serverless function (Web API) |
| `vc:fn:edge` | Edge function (Vercel /api route) |
| `vc:fn:streaming` | Streaming edge function |
| `vc:fn:config:node` | Function config (Node runtime) |
| `vc:fn:config:edge` | Function config (Edge runtime) |
| `vc:fn:config:region` | Function config with region |
| `vc:fn:config:duration` | Function config with maxDuration |
| `vc:fn:get` | GET handler |
| `vc:fn:post` | POST handler |
| `vc:fn:crud` | Multi-method handler (GET/POST/PUT/DELETE) |
| `vc:fn:json` | JSON response |
| `vc:fn:error` | Error response |
| `vc:fn:geo` | Geolocation from request |
| `vc:fn:waituntil` | waitUntil for background work |
| `vc:fn:cors` | CORS headers helper |
| `vc:fn:redirect` | Redirect response |
| `vc:fn:cookies` | Cookie handling |
| `vc:fn:params` | URL search params extraction |
| `vc:fn:blob` | Vercel Blob upload |

### Next.js + Vercel Patterns (`vc:next:*`) — 30 snippets

| Trigger | Description |
|---------|-------------|
| `vc:next:isr` | ISR with revalidate |
| `vc:next:isr:demand` | On-demand ISR revalidation |
| `vc:next:isr:tag` | Tag-based revalidation |
| `vc:next:dynamic` | Dynamic route with generateStaticParams |
| `vc:next:image` | Next/Image optimized component |
| `vc:next:image:remote` | Next/Image remote pattern config |
| `vc:next:og` | OG image generation |
| `vc:next:middleware` | Middleware with matcher |
| `vc:next:middleware:geo` | Middleware with geo-redirect |
| `vc:next:middleware:auth` | Middleware auth check |
| `vc:next:middleware:rewrite` | Middleware rewrite |
| `vc:next:route` | App Router route handler |
| `vc:next:route:stream` | Streaming route handler |
| `vc:next:action` | Server action |
| `vc:next:server` | Async server component |
| `vc:next:loading` | Loading UI (Suspense) |
| `vc:next:error` | Error boundary |
| `vc:next:not:found` | Not found page |
| `vc:next:layout` | Root layout |
| `vc:next:metadata` | Metadata export |
| `vc:next:metadata:dynamic` | Dynamic generateMetadata |
| `vc:next:sitemap` | Sitemap generation |
| `vc:next:robots` | Robots.txt generation |
| `vc:next:analytics` | Vercel Analytics component |
| `vc:next:speed` | Speed Insights component |
| `vc:next:ppr` | Partial Prerendering (experimental) |
| `vc:next:cache` | Fetch with cache/revalidate |
| `vc:next:headers` | headers() and cookies() |
| `vc:next:redirect` | redirect() in server component |
| `vc:next:edge:config` | Edge Config read |

### Environment & Config (`vc:env:*`) — 10 snippets

| Trigger | Description |
|---------|-------------|
| `vc:env:check` | VERCEL env var check |
| `vc:env:url` | Base URL from VERCEL_URL |
| `vc:env:environment` | VERCEL_ENV check |
| `vc:env:region` | VERCEL_REGION usage |
| `vc:env:git` | VERCEL_GIT_* env vars |
| `vc:env:dotenv` | .env.local template |
| `vc:env:conditional` | Environment-conditional config |
| `vc:env:edge:config` | Edge Config client init |
| `vc:env:flags` | Feature flags via Edge Config |
| `vc:env:unstable:cache` | unstable_cache for data caching |

### Storage (`vc:store:*`) — 10 snippets

| Trigger | Description |
|---------|-------------|
| `vc:store:redis:init` | Upstash Redis client init |
| `vc:store:redis:get` | Redis get value |
| `vc:store:redis:set` | Redis set value with TTL |
| `vc:store:postgres:query` | Neon Postgres query |
| `vc:store:postgres:pool` | Neon Postgres connection pool |
| `vc:store:postgres:drizzle` | Neon Postgres with Drizzle ORM |
| `vc:store:blob:upload` | Vercel Blob upload |
| `vc:store:blob:list` | Vercel Blob list |
| `vc:store:blob:delete` | Vercel Blob delete |
| `vc:store:blob:client` | Vercel Blob client-side upload |

### AI SDK (`vc:ai:*`) — 5 snippets

| Trigger | Description |
|---------|-------------|
| `vc:ai:generate` | AI text generation |
| `vc:ai:stream` | AI streaming response |
| `vc:ai:chat` | AI chat component (useChat) |
| `vc:ai:embed` | AI embeddings |
| `vc:ai:tool` | AI tool calling |

### Deployment & CI (`vc:deploy:*`) — 15 snippets

| Trigger | Description |
|---------|-------------|
| `vc:deploy:cli` | Deploy via Vercel CLI |
| `vc:deploy:github` | GitHub Actions deploy workflow |
| `vc:deploy:ignore` | Ignore build step script |
| `vc:deploy:monorepo` | Monorepo project config |
| `vc:deploy:output:config` | Build Output API config.json |
| `vc:deploy:output:static` | Build Output API static route |
| `vc:deploy:output:function` | Build Output API serverless function |
| `vc:deploy:output:edge` | Build Output API edge function |
| `vc:deploy:domain:redirect` | Domain redirect (www to apex) |
| `vc:deploy:protection` | Deployment protection bypass |
| `vc:deploy:skew` | Skew protection config |
| `vc:deploy:next:config` | next.config.js for Vercel |
| `vc:deploy:turbo` | turbo.json for monorepo |
| `vc:deploy:webhook` | Deploy hook trigger |
| `vc:deploy:cron` | Cron job handler with CRON_SECRET |

## Links

- [Package Control](https://packagecontrol.io/packages/Vercel)
- [GitHub](https://github.com/renzojohnson/Vercel)
- [Issues](https://github.com/renzojohnson/Vercel/issues)
- [Author](https://renzojohnson.com)

## License

MIT License. Copyright (c) 2026 [Renzo Johnson](https://renzojohnson.com).
