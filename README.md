# Moonlight RSVP

Moonlight RSVP is the recommended FuseKit Hacker News demo app.

It is intentionally small but real-world enough to prove the product:

- Vite + Vercel Functions app for deployment
- custom domain in `vercel.json`
- Resend dependency and env usage
- RSVP API route that sends confirmation email
- webhook route protected by `WEBHOOK_SECRET`
- no committed raw secrets

## Expected FuseKit Inference

From this repo, FuseKit should infer:

- GitHub repo setup
- Vercel project/env/deploy setup
- Cloudflare DNS for `moonlite.rsvp`
- Resend provider pack
- webhook secret generation
- live URL verification

Run from the FuseKit repo:

```zsh
fusekit acceptance run examples/hn-demo-app --mode rehearsal
```

For the real recording, copy this app into a disposable GitHub repo and replace
`moonlite.rsvp` with the domain you control if you are not using the official demo domain.
