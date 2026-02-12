# Custom Domain Setup Guide for White AI Solutions

> **Current URL:** https://ai-automation-landing-mu.vercel.app
> **Hosting:** Vercel (free Hobby tier)
> **Date researched:** February 12, 2026

---

## Table of Contents

1. [Domain Registrar Comparison](#1-domain-registrar-comparison)
2. [Domain Name Availability](#2-domain-name-availability)
3. [Recommendation](#3-recommendation)
4. [Purchase Instructions](#4-purchase-instructions)
5. [Vercel Custom Domain Setup](#5-vercel-custom-domain-setup)
6. [Site Config Updates After Domain Is Live](#6-site-config-updates-after-domain-is-live)
7. [Cost Summary](#7-cost-summary)

---

## 1. Domain Registrar Comparison

### .com Domain Pricing (as of Feb 2026)

| Registrar | First Year | Renewal/yr | Free WHOIS Privacy | Notes |
|-----------|-----------|------------|---------------------|-------|
| **Cloudflare Registrar** | ~$10.44 | ~$10.44 | Yes | At-cost pricing (no markup). Same price every year. Includes free DNS, CDN, and SSL. |
| **Porkbun** | $11.08 | $11.08 | Yes | Consistent pricing, no bait-and-switch. Free email forwarding, URL forwarding, SSL. |
| **Namecheap** | ~$10.98 (standard) / ~$6.49-$9.98 (promo) | ~$13.98 | Yes | Cheap first year with promos, but renewal is ~30% higher. ICANN fee of $0.20 added at checkout. |
| **Squarespace Domains** | ~$20.00 | ~$20.00 | Yes | Most expensive option. Inherited Google Domains but raised prices. Not competitive for budget use. |

### Other TLD Pricing (Cloudflare at-cost)

| TLD | Registration | Renewal |
|-----|-------------|---------|
| .com | $10.44 | $10.44 |
| .dev | $10.18 | $10.18 |
| .solutions | $24.20 | $24.20 |

### Registrar Verdicts

- **Cloudflare Registrar** -- Best overall value. At-cost pricing with zero markup means your renewal price equals your registration price, year after year. The .com wholesale price from Verisign is currently ~$10.44 and Cloudflare passes it through at exactly that. You also get their world-class DNS, CDN, and DDoS protection for free. The only downside: the registrar UI is more bare-bones than Namecheap or Porkbun.

- **Porkbun** -- Close second. Transparent pricing at $11.08/yr for .com (both registration and renewal). Slightly more expensive than Cloudflare but has a friendlier UI, great customer support, and includes extras like email forwarding. Good alternative if you want a simpler purchasing experience.

- **Namecheap** -- Tempting first-year promos ($6.49-$9.98) but renewal jumps to ~$13.98/yr. Over 3 years, you pay more than Cloudflare or Porkbun. Still a solid registrar with good UI and support, but the renewal markup hurts on a tight budget.

- **Squarespace Domains** -- Not recommended. At $20/yr for .com, it is roughly double the cost of Cloudflare for the same domain. No reason to use this unless you are already deep in the Squarespace ecosystem.

---

## 2. Domain Name Availability

Availability checked via DNS lookups (dig SOA/NS/A records) and InstantDomainSearch on February 12, 2026.

| Domain | Available? | TLD Price (Cloudflare) | Notes |
|--------|-----------|----------------------|-------|
| **whiteaisolutions.com** | Yes | $10.44/yr | Clean, professional, matches the brand exactly. Top pick. |
| **whiteai.dev** | Yes | $10.18/yr | Shorter, techy feel. Good for a dev-focused brand. Slightly cheaper than .com. |
| **jonathanwhiteai.com** | Yes | $10.44/yr | Personal brand angle. Good if you want your name front and center. |
| **white-ai.com** | **No** | -- | Registered (Azure DNS nameservers active). Not available. |
| **whiteai.solutions** | Yes | $24.20/yr | Available but .solutions TLD is expensive ($24.20/yr) and uncommon. Not recommended. |
| **whiteaisolutions.dev** | Yes | $10.18/yr | Available. Same brand, .dev TLD, slightly cheaper. |
| **whiteautomation.com** | **No** | -- | Registered (NameBright DNS). Not available. |
| **whiteai.co** | **No** | -- | Registered (Afternic/GoDaddy). Likely parked for resale. |
| **whiteai.agency** | Yes | TBD | Available. .agency TLD may be pricier, less commonly recognized. |
| **whiteai.tech** | Yes | TBD | Available. .tech is recognizable but less authoritative than .com. |
| **getwhiteai.com** | Yes | $10.44/yr | Available. Actionable name, but longer. |
| **hirewhiteai.com** | Yes | $10.44/yr | Available. Good call-to-action domain, but long. |

### Top 3 Recommendations (Ranked)

1. **whiteaisolutions.com** -- Matches the business name exactly. Professional, memorable, and uses the trusted .com TLD. Clients searching for "White AI Solutions" will find this instantly. This is the correct choice.

2. **whiteai.dev** -- Shorter and clean. The .dev TLD signals technical credibility. Good alternative if you want brevity, but .com is more universally recognized by small business owners (your target audience).

3. **jonathanwhiteai.com** -- Strong personal brand play. Useful if you plan to be the face of the business long-term. Longer to type, but clear and professional.

---

## 3. Recommendation

**Buy `whiteaisolutions.com` from Cloudflare Registrar for $10.44/year.**

Reasons:
- Exact brand match (White AI Solutions)
- .com is the most trusted TLD for small business clients
- Cloudflare at-cost pricing means no renewal surprise ($10.44 every year)
- Free DNS, CDN, DDoS protection, and WHOIS privacy included
- Total annual cost: $10.44 (domain) + $0 (Vercel Hobby) = **$10.44/year**

If Cloudflare's registration interface feels too bare-bones, Porkbun is a great alternative at $11.08/yr with a friendlier UI. The $0.64/yr difference is negligible.

---

## 4. Purchase Instructions

### Option A: Cloudflare Registrar (Recommended)

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/) and sign up for a free account (if you don't have one)
2. In the left sidebar, click **Domain Registration** > **Register Domains**
3. Search for `whiteaisolutions.com`
4. Click **Purchase** and complete checkout ($10.44)
5. The domain will be added to your Cloudflare account with DNS already managed by Cloudflare

### Option B: Porkbun (Alternative)

1. Go to [porkbun.com](https://porkbun.com/) and create an account
2. Search for `whiteaisolutions.com`
3. Add to cart and complete checkout ($11.08)
4. Domain will be registered with Porkbun DNS management

---

## 5. Vercel Custom Domain Setup

### Step 1: Add the Domain in Vercel

1. Log in to [Vercel Dashboard](https://vercel.com/dashboard)
2. Select the **ai-automation-landing** project
3. Go to **Settings** tab > **Domains** in the left sidebar
4. Type `whiteaisolutions.com` in the domain input field
5. Click **Add**
6. Vercel will prompt you to also add `www.whiteaisolutions.com` -- accept this (it will redirect www to the apex domain)

### Step 2: Configure DNS Records

Vercel will show you the DNS records you need to add. The typical setup is:

#### For the apex domain (whiteaisolutions.com):

| Record Type | Name/Host | Value | TTL |
|-------------|-----------|-------|-----|
| **A** | `@` | `76.76.21.21` | Auto / 300 |

> Note: Vercel may provide a different IP address specific to your project. Use the IP shown in your Vercel dashboard. The legacy IP `76.76.21.21` continues to work, but Vercel now assigns optimized Anycast IPs per project for better performance.

#### For the www subdomain (www.whiteaisolutions.com):

| Record Type | Name/Host | Value | TTL |
|-------------|-----------|-------|-----|
| **CNAME** | `www` | `cname.vercel-dns.com.` | Auto / 300 |

> Note: Vercel may show a project-specific CNAME value like `d1d4fc829fe7bc7c.vercel-dns-017.com`. Use whatever value Vercel's dashboard displays -- it is unique to your project.

### Step 3: Add DNS Records at Your Registrar

#### If using Cloudflare:

1. In [Cloudflare Dashboard](https://dash.cloudflare.com/), select the domain `whiteaisolutions.com`
2. Go to **DNS** > **Records**
3. Click **Add record**
4. Add the **A record**:
   - Type: `A`
   - Name: `@`
   - IPv4 address: `76.76.21.21` (or the IP from Vercel dashboard)
   - Proxy status: **DNS only (gray cloud)** -- important! Set to "DNS only", not "Proxied"
   - TTL: Auto
5. Add the **CNAME record**:
   - Type: `CNAME`
   - Name: `www`
   - Target: `cname.vercel-dns.com` (or the value from Vercel dashboard)
   - Proxy status: **DNS only (gray cloud)**
   - TTL: Auto

> **IMPORTANT:** When using Cloudflare with Vercel, set the proxy status to "DNS only" (gray cloud icon, NOT orange). Cloudflare's proxy can interfere with Vercel's SSL certificate provisioning and edge routing. You can enable Cloudflare proxy later after the domain is verified, but start with DNS only.

#### If using Porkbun:

1. Log in to [Porkbun](https://porkbun.com/) and go to **Domain Management**
2. Click the domain `whiteaisolutions.com`
3. Go to the **DNS Records** section
4. Delete any default records (parking records, etc.)
5. Add the **A record**:
   - Host: (leave blank for apex)
   - Type: `A`
   - Answer: `76.76.21.21` (or the IP from Vercel dashboard)
   - TTL: 300
6. Add the **CNAME record**:
   - Host: `www`
   - Type: `CNAME`
   - Answer: `cname.vercel-dns.com` (or the value from Vercel dashboard)
   - TTL: 300

### Step 4: Wait for DNS Propagation

- DNS changes typically take **5-30 minutes** to propagate, but can take up to 48 hours in rare cases
- You can check propagation status at [dnschecker.org](https://dnschecker.org/) by looking up your domain
- Vercel's dashboard will show a green checkmark once the domain is verified

### Step 5: Verify SSL Certificate

1. Go back to **Vercel Dashboard** > your project > **Settings** > **Domains**
2. Both `whiteaisolutions.com` and `www.whiteaisolutions.com` should show as **Valid Configuration** with green checkmarks
3. Vercel automatically provisions a free SSL certificate (Let's Encrypt) -- no action needed
4. Visit `https://whiteaisolutions.com` in your browser and verify:
   - The site loads correctly
   - The padlock icon shows in the address bar (SSL active)
   - `www.whiteaisolutions.com` redirects to `whiteaisolutions.com` (or vice versa, per your preference)

### Step 6: Verify the Old URL Redirects

After the custom domain is active, the original `ai-automation-landing-mu.vercel.app` URL will continue to work. Vercel does not automatically redirect it. This is fine -- search engines will follow your canonical URL tag (which you will update in Step 6 below).

---

## 6. Site Config Updates After Domain Is Live

Once `whiteaisolutions.com` (or your chosen domain) is verified and working, update these files to replace all references to the old Vercel URL.

### Files to Update

Replace all instances of:
```
https://ai-automation-landing-mu.vercel.app
```
with:
```
https://whiteaisolutions.com
```

#### 1. `astro.config.mjs` -- Site URL for sitemap generation

**File:** `astro.config.mjs` (project root)
**Line 8:** Change the `site` property

```js
// Before
site: 'https://ai-automation-landing-mu.vercel.app',

// After
site: 'https://whiteaisolutions.com',
```

#### 2. `src/layouts/Layout.astro` -- Canonical URL, OG tags, structured data

**File:** `src/layouts/Layout.astro`

Update these lines:
- **Line 31** (og:url): `content="https://whiteaisolutions.com"`
- **Line 32** (og:image): `content="https://whiteaisolutions.com/og-image.svg"`
- **Line 42** (twitter:image): `content="https://whiteaisolutions.com/og-image.svg"`
- **Line 45** (canonical): `href="https://whiteaisolutions.com"`
- **Line 60** (Schema.org url): `"url": "https://whiteaisolutions.com"`

#### 3. `public/robots.txt` -- Sitemap URL

**File:** `public/robots.txt`
**Line 3:** Update the sitemap URL

```
Sitemap: https://whiteaisolutions.com/sitemap-index.xml
```

### Quick Reference: All Occurrences

| File | Line(s) | What to Update |
|------|---------|---------------|
| `astro.config.mjs` | 8 | `site` property |
| `src/layouts/Layout.astro` | 31 | `og:url` meta tag |
| `src/layouts/Layout.astro` | 32 | `og:image` meta tag |
| `src/layouts/Layout.astro` | 42 | `twitter:image` meta tag |
| `src/layouts/Layout.astro` | 45 | `canonical` link tag |
| `src/layouts/Layout.astro` | 60 | Schema.org `url` property |
| `public/robots.txt` | 3 | `Sitemap` directive |

**Total: 7 occurrences across 3 files.**

After making these changes, commit and push. Vercel will auto-deploy with the updated URLs.

---

## 7. Cost Summary

### Annual Cost Breakdown

| Item | Cost |
|------|------|
| Domain (whiteaisolutions.com via Cloudflare) | $10.44/yr |
| Hosting (Vercel Hobby tier) | $0/yr |
| SSL Certificate (Vercel auto-provisioned) | $0/yr |
| DNS hosting (Cloudflare) | $0/yr |
| WHOIS Privacy (Cloudflare) | $0/yr |
| **Total annual cost** | **$10.44/yr** |

### First 3 Months Estimated Cost

Since domain registration is annual (no monthly option), the upfront cost is:

| Item | Cost |
|------|------|
| Domain registration (1 year minimum) | $10.44 |
| Everything else | $0 |
| **Total to get started** | **$10.44** |

That is the entire cost to go from `ai-automation-landing-mu.vercel.app` to `whiteaisolutions.com` with full SSL, CDN, and professional DNS.

---

## Sources

- [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/) -- At-cost domain pricing
- [Cloudflare Domain Pricing Tracker](https://cfdomainpricing.com/) -- Current TLD prices at Cloudflare
- [Porkbun Domain Pricing](https://porkbun.com/products/domains) -- Registration and renewal prices
- [Namecheap .com Registration](https://www.namecheap.com/domains/registration/gtld/com/) -- .com pricing and promos
- [Squarespace Domains](https://domains.squarespace.com/) -- Post-Google Domains pricing
- [Vercel: Adding a Custom Domain](https://vercel.com/docs/domains/working-with-domains/add-a-domain) -- Official setup guide
- [Vercel: Working with DNS](https://vercel.com/docs/domains/working-with-dns) -- DNS configuration reference
- [Vercel: A Record and CAA](https://vercel.com/kb/guide/a-record-and-caa-with-vercel) -- A record IP details
