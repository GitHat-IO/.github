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

**API:** api.githat.io — 86 Lambda functions

**Database:** DynamoDB (16 tables)

**Email:** SES (noreply@githat.io)

**Monitoring:** CloudWatch (3 alarms)

---

### Repositories

- [**MicroFrontEnds**](https://github.com/GitHat-IO/MicroFrontEnds) — Dashboard, SDK, frontend
- [**MicroBackEnds**](https://github.com/GitHat-IO/MicroBackEnds) — Lambda API, DynamoDB
- [**create-githat-app**](https://github.com/GitHat-IO/create-githat-app) — CLI (npm)

---

<div align="center">

[Website](https://githat.io) • [SDK](https://www.npmjs.com/package/@githat/nextjs) • [CLI](https://www.npmjs.com/package/create-githat-app) • [Docs](https://githat.io/docs)

© 2026 GitHat Inc.

</div>
