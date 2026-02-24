<div align="center">

# GitHat

**Auth + Hosting • Replaces Clerk + Vercel**

[![SDK](https://img.shields.io/npm/v/@githat/nextjs?style=flat-square&logo=npm&logoColor=white&label=%40githat%2Fnextjs&color=cb3837)](https://www.npmjs.com/package/@githat/nextjs)
[![CLI](https://img.shields.io/npm/v/create-githat-app?style=flat-square&logo=npm&logoColor=white&label=create-githat-app&color=cb3837)](https://www.npmjs.com/package/create-githat-app)
[![Website](https://img.shields.io/website?style=flat-square&url=https%3A%2F%2Fgithat.io&up_message=live&up_color=1f6feb&label=githat.io)](https://githat.io)

</div>

---

Pre-built sign-in UI • JWT tokens • Slug-based hosting at `slug.githat.io` • **Bring your own database**

```bash
npx create-githat-app my-app
cd my-app && npm run dev
```

---

### SDK

```bash
npm install @githat/nextjs
```

**Components:** `SignInForm` `SignUpForm` `ForgotPasswordForm` `UserButton` `OrgSwitcher`

**Hooks:** `useAuth()` `useData()` `useGitHat()`

**Server:** `verifyToken()` `withAuth()` `getAuth()`

Next.js 14-16 • Middleware/Proxy • Cookie or localStorage • Auto token refresh

---

### CLI

```bash
npx create-githat-app my-app
```

Next.js 14-16 App Router • Auth pages • Password reset • Dashboard • Team invites • TypeScript + Tailwind

---

### Infrastructure

**Frontend:** CloudFront + S3 at githat.io

**API:** api.githat.io — 95 Lambda functions

**Database:** DynamoDB (18 tables)

**Email:** SES (noreply@githat.io)

**Monitoring:** CloudWatch (3 alarms)

---

### Repositories

- [**MicroFrontEnds**](https://github.com/GitHat-IO/MicroFrontEnds) — Dashboard, SDK, frontend
- [**MicroBackEnds**](https://github.com/GitHat-IO/MicroBackEnds) — Lambda API, DynamoDB
- [**create-githat-app**](https://github.com/GitHat-IO/create-githat-app) — CLI (npm)

---

---

### Documentation

[Quick Start](https://githat.io/docs/quickstart) •
[SDK Reference](https://githat.io/docs/sdk) •
[API Reference](https://githat.io/docs/api) •
[CLI](https://githat.io/docs/cli) •
[MCP Servers](https://githat.io/docs/mcp) •
[AI Agents](https://githat.io/docs/agents) •
[BYOD](https://githat.io/docs/byod) •
[Customer Data API](https://githat.io/docs/data) •
[Skills Marketplace](https://githat.io/docs/skills)

**Framework Guides:**
[Next.js](https://githat.io/docs/nextjs) •
[React](https://githat.io/docs/react) •
[Node.js](https://githat.io/docs/node) •
[Python](https://githat.io/docs/python) •
[Flask](https://githat.io/docs/flask) •
[FastAPI](https://githat.io/docs/fastapi)

**Tutorials:**
[Next.js Auth Guide](https://githat.io/guides/nextjs-authentication) •
[React Auth Guide](https://githat.io/guides/react-authentication) •
[Node.js Auth Guide](https://githat.io/guides/node-authentication) •
[Multi-Tenant Auth](https://githat.io/guides/multi-tenant-auth) •
[Clerk Migration](https://githat.io/docs/clerk-migration)

**Compare:**
[vs Clerk](https://githat.io/compare/githat-vs-clerk) •
[vs Auth0](https://githat.io/compare/githat-vs-auth0) •
[vs Firebase](https://githat.io/compare/githat-vs-firebase) •
[vs Supabase](https://githat.io/compare/githat-vs-supabase) •
[vs Vercel](https://githat.io/compare/githat-vs-vercel)

---

<div align="center">

[Website](https://githat.io) • [Pricing](https://githat.io/pricing) • [Docs](https://githat.io/docs) • [SDK](https://www.npmjs.com/package/@githat/nextjs) • [CLI](https://www.npmjs.com/package/create-githat-app)

© 2026 GitHat Inc.

</div>
