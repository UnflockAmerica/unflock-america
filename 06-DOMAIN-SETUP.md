# UNFLOCK AMERICA — DOMAIN & HOSTING SETUP GUIDE
## OPSEC-Max Instructions

---

## 1. BUY THE DOMAIN (Njalla — Most OPSEC)

**Why Njalla:** They are the registrar of record. Your name never appears in WHOIS. They accept Bitcoin and Monero.

**Steps:**
1. Go to **njalla.com** over Tor or VPN (not your home IP)
2. Search for available domains:
   - `unflockamerica.com` (best)
   - `unflock.us`
   - `unflock.help`
   - `projectunchain.org`
   - `flockban.org`
3. Purchase with **Bitcoin** (not credit card)
4. Use the ProtonMail: **unflock.now@proton.me**
5. Set nameservers to Cloudflare (free plan) — or use Njalla's DNS

**Fallback (Namecheap):**
- Go to namecheap.com over Tor/VPN
- Search for same domains
- Purchase with Bitcoin
- WHOIS privacy is free (toggle it on)

---

## 2. SET UP CLOUDFLARE DNS (Free)

1. Create a Cloudflare account using `unflock.now@proton.me`
2. Add the domain you purchased
3. Cloudflare will give you nameservers — set these at Njalla/Namecheap
4. In Cloudflare DNS, add:
   - `A` record → `185.199.108.153` (GitHub Pages IP)
   - `A` record → `185.199.109.153`
   - `A` record → `185.199.110.153`
   - `A` record → `185.199.111.153`
   - `AAAA` record → `2606:50c0:8000::153` (IPv6)
   - `AAAA` record → `2606:50c0:8001::153`
   - `AAAA` record → `2606:50c0:8002::153`
   - `AAAA` record → `2606:50c0:8003::153`
   - `CNAME` record → `www` → `unflockamerica.github.io`
5. Enable proxy (orange cloud) for security

---

## 3. CONNECT TO GITHUB PAGES

1. Go to `https://github.com/UnflockAmerica/unflock-america/settings/pages`
2. Under "Custom domain", enter your domain (e.g. `unflockamerica.com`)
3. Click Save
4. Check "Enforce HTTPS"

---

## 4. VERIFY

1. Wait up to 10 minutes for DNS propagation
2. Visit `https://unflockamerica.com` — should show the UnFlock America landing page
3. Visit `https://unflockamerica.com/01-MODEL-ORDINANCE.md` — should show the ordinance

---

## 5. OPSEC REMINDERS

- **Never** access the Njalla/Cloudflare/GitHub accounts from your home IP
- Use Tor or a VPN for all admin access
- **Never** use your personal name, address, or phone number
- Use `unflock.now@proton.me` for everything
- Pay for domain with Bitcoin from a non-KYC source
- No analytics, no tracking, no forms on the site — it's purely informational

---

*Current site (before custom domain):* **https://unflockamerica.github.io**