<div align="center">

# GitHat

**The clerk at the door of your app.**

Identity + edge for the apps that don't want to glue ten vendors together. Bring your own database.

[**🌐 githat.io**](https://githat.io)&nbsp;&nbsp;·&nbsp;&nbsp;[**📦 npx create-githat-app**](https://github.com/GitHat-IO/create-githat-app)&nbsp;&nbsp;·&nbsp;&nbsp;[**🔌 api.githat.io**](https://api.githat.io)

</div>

---

## What GitHat is

One install. Sign-in, sign-up, password reset, social, passkeys, 2FA, organizations, audit log — wired up. Hosting too, when you want it.

- **Auth** — verified locally, no shared secrets between issuer and consumers
- **Edge** — managed certs, locked to a single CA, auto-rotates
- **SDK** — drop-in for modern fullstack
- **Platform** — one auth surface, many apps under it

## The fleet

GitHat is the identity layer. Every app in the platform delegates auth to `api.githat.io`:

<!-- IDENTITY:fleet_table -->
| App | Domain | Org |
|---|---|---|
| **Sebastn** — payments rail | [sebastn.com](https://sebastn.com) | [SebasTN-Rhys](https://github.com/SebasTN-Rhys) |
| **ClickReserv** — booking SaaS, 56 templates | [reserv.click](https://reserv.click) | [ClickReserv](https://github.com/ClickReserv) |
| **Quantl** — quant signals + forecasting | [quantl.click](https://quantl.click) | [QuantLinc](https://github.com/QuantLinc) |
| **Colmado** — neighborhood commerce | [colmado.click](https://colmado.click) | [Colmado-Inc](https://github.com/Colmado-Inc) |
| **NFTeria** — web4 identity + agents | [nfteria.click](https://nfteria.click) | [NFTeria](https://github.com/NFTeria) |
<!-- /IDENTITY:fleet_table -->

## Get started

```bash
npx create-githat-app my-app
cd my-app && npm run dev
```

That's it.

## Security posture

- ✅ Verified domains (`githat.io`, `www.githat.io`)
- ✅ Tokens verified locally — no shared secrets
- ✅ Per-app audience enforcement (no cross-tenant replay)
- ✅ Certs locked to a single CA at the apex
- ✅ Required 2FA, signed commits, branch protection, secret scanning

## Contact

Security: [security@githat.io](mailto:security@githat.io) — see [SECURITY.md](https://github.com/GitHat-IO/.github/blob/main/SECURITY.md)
Support: [hello@githat.io](mailto:hello@githat.io)
Status: [status.githat.io](https://status.githat.io)
