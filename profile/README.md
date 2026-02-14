<div align="center">

<!-- 3D Wave Header -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:1f6feb&height=230&section=header&text=GitHat&fontColor=ffffff&fontSize=90&fontAlignY=32&desc=Identity%20Infrastructure%20for%20Modern%20Apps&descSize=22&descAlignY=56&descColor=58a6ff&animation=fadeIn&stroke=58a6ff&strokeWidth=1" width="100%" alt="GitHat"/>

<br/>

<!-- Logo -->
<img src="githat-logo.png" width="180" alt="GitHat Logo"/>

<br/><br/>

<!-- Animated Typing -->
<a href="https://githat.io">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=80&lines=Authentication+%C2%B7+Organizations+%C2%B7+Teams;Ship+identity+in+minutes%2C+not+months." alt="Typing SVG"/>
</a>

<br/>

<!-- Badges -->
<a href="https://www.npmjs.com/package/@githat/nextjs">
  <img src="https://img.shields.io/npm/v/@githat/nextjs?style=for-the-badge&logo=npm&logoColor=white&label=%40githat%2Fnextjs&color=cb3837" alt="SDK Version"/>
</a>
&nbsp;
<a href="https://www.npmjs.com/package/create-githat-app">
  <img src="https://img.shields.io/npm/v/create-githat-app?style=for-the-badge&logo=npm&logoColor=white&label=create-githat-app&color=cb3837" alt="CLI Version"/>
</a>
&nbsp;
<a href="https://githat.io">
  <img src="https://img.shields.io/website?style=for-the-badge&url=https%3A%2F%2Fgithat.io&up_message=live&up_color=1f6feb&label=githat.io&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiLz48bGluZSB4MT0iMiIgeTE9IjEyIiB4Mj0iMjIiIHkyPSIxMiIvPjxwYXRoIGQ9Ik0xMiAyYTE1LjMgMTUuMyAwIDAgMSA0IDEwIDE1LjMgMTUuMyAwIDAgMS00IDEwIDE1LjMgMTUuMyAwIDAgMS00LTEwIDE1LjMgMTUuMyAwIDAgMSA0LTEweiIvPjwvc3ZnPg==" alt="Website"/>
</a>

</div>

<br/>

---

<br/>

## What is GitHat?

**GitHat** provides complete identity infrastructure so you can add authentication, organization management, and team collaboration to any app in minutes. Drop in the SDK, run the CLI, and ship — sign-up, sign-in, email verification, multi-org switching, role-based access, and API key management all work out of the box.

```bash
npx create-githat-app my-app
```

<br/>

---

<br/>

## Packages

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">
        <a href="https://www.npmjs.com/package/@githat/nextjs">@githat/nextjs</a>
      </h3>
      <p align="center">
        <code>npm install @githat/nextjs</code>
      </p>
      <p>Full-featured React SDK for Next.js applications.</p>
      <ul>
        <li><code>&lt;SignInForm /&gt;</code> &mdash; branded sign-in</li>
        <li><code>&lt;SignUpForm /&gt;</code> &mdash; registration + email verify</li>
        <li><code>&lt;UserButton /&gt;</code> &mdash; avatar dropdown</li>
        <li><code>&lt;OrgSwitcher /&gt;</code> &mdash; multi-org selector</li>
        <li><code>useAuth()</code> &mdash; session state hook</li>
        <li><code>useOrg()</code> &mdash; organization context hook</li>
        <li>Next.js middleware &mdash; route protection</li>
        <li>Auto token refresh &mdash; seamless sessions</li>
        <li>CSS theme &mdash; <code>@githat/nextjs/styles</code></li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3 align="center">
        <a href="https://www.npmjs.com/package/create-githat-app">create-githat-app</a>
      </h3>
      <p align="center">
        <code>npx create-githat-app</code>
      </p>
      <p>Interactive CLI that scaffolds a complete project.</p>
      <ul>
        <li>Next.js 14+ App Router template</li>
        <li>Auth pages &mdash; sign-in, sign-up, verify</li>
        <li>Protected dashboard layout</li>
        <li>API client with retry logic</li>
        <li>Organization management UI</li>
        <li>Team invite flow</li>
        <li>TypeScript + Tailwind CSS</li>
        <li><code>.env</code> pre-configured</li>
        <li>Production-ready from day one</li>
      </ul>
    </td>
  </tr>
</table>

<br/>

---

<br/>

## Built With

<div align="center">

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=react,nextjs,ts,nodejs,aws,dynamodb&theme=dark" alt="Tech Stack"/>
</a>

<br/><br/>

**React** &middot; **Next.js** &middot; **TypeScript** &middot; **Node.js** &middot; **AWS Lambda** &middot; **DynamoDB**

</div>

<br/>

---

<br/>

## Architecture

```text
 ╔══════════════════════════════════════════════════════╗
 ║                    githat.io                        ║
 ║               CloudFront + S3                       ║
 ╠══════════════════════════════════════════════════════╣
 ║                                                     ║
 ║   @githat/nextjs SDK             Dashboard          ║
 ║   ┌────────────────┐      ┌───────────────────┐    ║
 ║   │  SignInForm     │      │  User Management  │    ║
 ║   │  SignUpForm     │      │  Org Settings     │    ║
 ║   │  UserButton     │      │  Team Invites     │    ║
 ║   │  OrgSwitcher    │      │  API Keys         │    ║
 ║   │  Middleware     │      │  Billing           │    ║
 ║   └───────┬────────┘      └────────┬──────────┘    ║
 ║           │                        │                ║
 ╠═══════════╧════════════════════════╧════════════════╣
 ║                  api.githat.io                      ║
 ║            API Gateway + 49 Lambdas                 ║
 ╠══════════════════════════════════════════════════════╣
 ║   DynamoDB (9 tables)  │   SES    │   CloudWatch   ║
 ╚══════════════════════════════════════════════════════╝
```

<br/>

---

<br/>

## Quick Start

```bash
# 1  Scaffold a new project
npx create-githat-app my-app

# 2  Add your publishable key
echo 'NEXT_PUBLIC_GITHAT_KEY=pk_live_your_key_here' > my-app/.env.local

# 3  Run
cd my-app && npm run dev
```

Or add the SDK to an existing Next.js app:

```bash
npm install @githat/nextjs
```

```tsx
import { GitHatProvider, SignInForm } from "@githat/nextjs";
import "@githat/nextjs/styles";

export default function App({ children }) {
  return (
    <GitHatProvider publishableKey={process.env.NEXT_PUBLIC_GITHAT_KEY!}>
      {children}
    </GitHatProvider>
  );
}
```

<br/>

---

<br/>

## Repositories

| Repo | Description |
| --- | --- |
| [MicroFrontEnds](https://github.com/GitHat-IO/MicroFrontEnds) | Dashboard, SDK, and frontend components |
| [MicroBackEnds](https://github.com/GitHat-IO/MicroBackEnds) | Lambda API, DynamoDB, auth handlers |
| [create-githat-app](https://github.com/GitHat-IO/create-githat-app) | CLI scaffolder (published to npm) |

<br/>

---

<br/>

<div align="center">

### Links

[Website](https://githat.io) &middot; [SDK on npm](https://www.npmjs.com/package/@githat/nextjs) &middot; [CLI on npm](https://www.npmjs.com/package/create-githat-app) &middot; [Contact](mailto:contact@githat.io)

<br/><br/>

<!-- 3D Wave Footer -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1f6feb,50:161b22,100:0d1117&height=130&section=footer&animation=fadeIn" width="100%" alt="Footer"/>

**&copy; 2026 GitHat Inc. All rights reserved.**

</div>
