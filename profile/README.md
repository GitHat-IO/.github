<div align="center">

# GitHat

**The clerk at the door of your app.**

Auth + hosting that replaces Clerk + Vercel. Bring your own database.

[**🌐 githat.io**](https://githat.io)&nbsp;&nbsp;·&nbsp;&nbsp;[**📦 npx create-githat-app**](https://github.com/GitHat-IO/create-githat-app)&nbsp;&nbsp;·&nbsp;&nbsp;[**🔌 api.githat.io**](https://api.githat.io)

</div>

---

## What GitHat is

GitHat is an identity + edge platform for SaaS apps that don't want to glue 10 vendors together. One install gives you:

- **Auth** — RS256 JWTs signed by AWS KMS, sessions in httpOnly cookies, audit-trail to a SOC2-compliant WORM bucket
- **Hosting** — Route 53 → CloudFront (ACM cert auto-rotation) → EC2 with Caddy + Node
- **SDK** — `@githat/nextjs` works in App Router, RSC, and middleware
- **Multi-app platform** — One auth surface, many apps under it (see the constellation below)

## The GitHat constellation

GitHat is the identity layer. Every app in the platform delegates auth to `api.githat.io`:

| App | Domain | Org |
|---|---|---|
| **Sebastn** — Stripe Connect, batteries included | [sebastn.com](https://sebastn.com) | [SebasTN-Rhys](https://github.com/SebasTN-Rhys) |
| **ClickReserv** — Booking SaaS, 56 templates | [reserv.click](https://reserv.click) | [ClickReserv](https://github.com/ClickReserv) |
| **Quantl** — ML pipeline + trading platform | [quantl.click](https://quantl.click) | [QuantLinc](https://github.com/QuantLinc) |
| **Colmado** — Neighborhood commerce | [colmado.click](https://colmado.click) | [Colmado-Inc](https://github.com/Colmado-Inc) |
| **NFTeria** — Web4 identity + agents | [nfteria.click](https://nfteria.click) | [NFTeria](https://github.com/NFTeria) |

## Get started in 30 seconds

```bash
npx create-githat-app my-app
cd my-app && npm run dev
```

That's it. You get sign-in, sign-up, password reset, OAuth (Google/GitHub/Apple/Microsoft/Discord/Slack/X), passkeys, 2FA, organizations, audit log — wired up.

## Security posture

- ✅ Verified domain (`githat.io`, `www.githat.io`) — see the badge above
- ✅ RS256 JWT signing via AWS KMS (no shared secrets between issuer and consumers)
- ✅ Token verification via public JWKS at `/.well-known/jwks.json` (5-min cache)
- ✅ Audience claim enforcement per-app (no cross-tenant token replay)
- ✅ CAA records lock cert issuance to AWS only
- ✅ SOC 2 CC7.2 audit archive (Object Lock COMPLIANCE 7y)
- ✅ Required 2FA, signed commits, branch protection, secret scanning

## Contact

Security: [security@githat.io](mailto:security@githat.io) — see [SECURITY.md](https://github.com/GitHat-IO/.github/blob/main/SECURITY.md)
Support: [hello@githat.io](mailto:hello@githat.io)
Status: [status.githat.io](https://status.githat.io)
