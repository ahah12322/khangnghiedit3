# Khang Page - Vercel Deploy

## Chay local

```bash
pnpm install
pnpm dev
```

## Deploy len Vercel

1. Push source len GitHub/GitLab/Bitbucket.
2. Vao Vercel, chon `Add New -> Project`.
3. Import repo nay.
4. Framework preset: `Next.js` (tu dong detect).
5. Build command: `pnpm build`.
6. Install command: `pnpm install`.
7. Output directory: de mac dinh.
8. Bam `Deploy`.

## Vercel Analytics

- Da tich hop package `@vercel/analytics`.
- Da gan `<Analytics />` trong root layout: `src/app/layout.tsx`.
- Khi deploy tren Vercel, metric se tu dong thu thap tren dashboard Analytics cua project.

## Luu y

- Endpoint `src/app/api/send/route.ts` dang hard-code TOKEN/CHAT_ID.
- Nen doi sang Environment Variables tren Vercel de an toan hon:
  - `TELEGRAM_BOT_TOKEN`
  - `TELEGRAM_CHAT_ID`
