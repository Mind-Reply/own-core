# OWNMODEL — Daily Production Checklist

## Morning (08:00 – 09:00)
- [ ] Run `DAILY_AGENT_OPS.bat`
- [ ] Run `Wire-All-Access.ps1`
- [ ] Open Gemini with OWNMODEL loaded
- [ ] Verify: `aurel.mind-reply.com` returns 200
- [ ] Check GitHub Actions for overnight failures

## Core Work (09:00 – 12:00)
- [ ] Active repo: `mind-reply`
- [ ] Primary model: Gemini
- [ ] Every commit: clean message + local test
- [ ] Push to `main` → Vercel auto-deploys

## Deploy Verification (after every push)
- [ ] `curl -I https://aurel.mind-reply.com` → 200
- [ ] No console errors in production
- [ ] GitHub Actions: deploy.yml passed

## Edge &amp; Router (12:00 – 15:00)
- [ ] WhatsApp router: webhook verified
- [ ] Cloudflare Workers: edge routes healthy
- [ ] LiteLLM gateway: port 4000 responding

## Database (15:00 – 17:00)
- [ ] Run Supabase audit (supabase-postgres-best-practices)
- [ ] Check indexes: GIN, BTREE on WHERE/JOIN columns
- [ ] Verify RLS policies

## End of Day (17:00 – 18:00)
- [ ] Run `Wire-All-Access.ps1`
- [ ] Open OWNMODEL Dashboard
- [ ] Update `ownmodel.yaml` with today's changes
- [ ] Push all repos
- [ ] Write end-of-day summary
