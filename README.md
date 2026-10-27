# TOF — TC’s creator connection

Independent 18+ creator-community frontend. Not affiliated with OnlyFans or Clapper.

## Run

Node 22.12+ recommended.

```sh
npm install
npm run dev
npm run check
npm run build
```

Deploy the generated `dist` directory on a static host. Camera preview needs HTTPS or localhost. No API keys are required for this prototype.

## Implemented

- Responsive discovery feed with category filters and locally saved likes.
- Creator profile, validated OnlyFans link and local post composer.
- Local camera preview with explicit permission and track cleanup.
- Local chat preview, virtual gift tray with demo credits only.
- Battle simulation with timer, scoring, reset and selectable duration.
- Co-host panel and explicit integration messages.
- Profile settings, local data clearing and session age notice.
- Escaping of user text before HTML rendering; link validation.

## Not production functionality

There are no registered accounts, public broadcasts, remote co-hosts, real viewers, real payments, payouts, persistent public chat or operational moderation. Demo credits have no monetary value. The age notice is self-attestation, not verified age assurance. Do not open production adult access based on this notice alone. No passwords or identity documents are collected.

## Backend work needed before launch

1. Auth, email verification, secure password recovery and role-based authorization.
2. Server-enforced adult verification and creator onboarding; store provider references rather than identity documents in the client.
3. Streaming rooms and short-lived, server-issued tokens; moderator permissions; host/guest consent and disconnect controls.
4. Database with row-level authorization for profiles, posts, followers, rooms, messages, reports and blocks.
5. Server-authoritative battle lifecycle, gift ledger, payment webhooks, refunds and payout reconciliation; never trust client balances or scores.
6. Moderation queues, reporting escalation, abuse prevention and content rules before public uploads or streaming.
7. Service and payment-provider compatibility review for the final content policy.

## Lovable

This repository was authored directly through GitHub without invoking Lovable generation. It is not connected to or hosted by Lovable. Lovable’s documented integration creates a repository from a Lovable project and does not import existing repositories: https://docs.lovable.dev/integrations/github . If a supported linked Lovable project becomes available, code can be adapted to its framework and linked repository without sending an AI build prompt.

## Privacy

Preview profile, posts and likes are stored in browser localStorage; age acknowledgement is stored in sessionStorage. Camera frames remain in the local video element and are not transmitted. Google Fonts is an optional external stylesheet request. Do not enter sensitive information in a local prototype.
