# 🍽️ MealWheelIQ

**Spin it. Cook it. Love it.**

An AI-powered family dinner planning app that eliminates the nightly "what's for dinner?" argument. Three modes, one AI chef, zero stress.

---

## Live URLs

| | URL |
|---|---|
| **Landing page** | https://mealwheeliq.com |
| **Sign in / Sign up** | https://mealwheeliq.com/login.html |
| **App** | https://mealwheeliq.com/app.html |
| **Blog** | https://mealwheeliq.com/blog/ |
| **API** | https://api.mealwheeliq.com |
| **API health check** | https://api.mealwheeliq.com/ |

---

## Three Ways to Spin

### 🧊 Tonight's Dinner
Spin the wheel, get 3 chef-quality recipes built from your actual pantry in seconds. Each spin lands on a cuisine style — American, Mediterranean, Chef's Special, Quick Meal, Comfort Food, and more. No extra shopping required.

### 📅 Plan My Week
Generate all 5 weeknight dinners in one shot. Each night is assigned a distinct cuisine style for real variety:
- **Monday** — Bold American / BBQ
- **Tuesday** — Mediterranean / Italian
- **Wednesday** — Light & Fresh (big salad, grain bowl, no-cook)
- **Thursday** — Asian-inspired
- **Friday** — Creative Wildcard

Includes a complete weekly grocery list sorted by category with a buy-by date and per-day ingredient labels. Share the list with your shopper via native share sheet. Use the **🔀 Mix Up** button on any night to swap to a different cuisine style (one mix-up per night per 24 hours).

### 🍲 Soup Creator ⭐ New
A dedicated soup mode that spins an 8-segment soup wheel and generates one cookbook-quality soup recipe from your pantry:

| Segment | Style |
|---|---|
| 🍜 Broth & Noodle | Ramen, pho, chicken noodle, udon |
| 🥣 Creamy & Blended | Bisque, butternut squash, tomato, potato leek |
| 🫕 Hearty Stew | Beef stew, lamb tagine, posole, Irish stew |
| 🌶️ Chili & Chowder | Beef chili, white chicken chili, corn chowder |
| 🌍 World Soups | Minestrone, borscht, miso, mulligatawny |
| 🥬 Light & Fresh | Lentil, tomato basil, vegetable, gazpacho |
| 🍄 Umami & Rich | French onion, mushroom, miso ramen, porcini |
| 🎲 Chef's Surprise | Bold, unexpected combinations |

Every soup recipe includes layered flavor building, proper simmer timing, and a finishing touch (fresh herbs, acid, garnish). After generation, tap **"🍲 Make it a big batch?"** to instantly scale to ×3 servings — perfect for meal prep.

---

## Core Features

### 📸 Pantry Scanning
Snap a photo of your fridge or pantry — Claude vision identifies everything in the image. Review and confirm items on a clean edit screen before saving. Client-side compression handles any phone camera size.

### 🎤 Voice & Text Craving Input
Tell the app what you're in the mood for before spinning. "Something spicy and Asian" or "light, nothing too heavy" — your craving takes priority over the wheel's category and shapes the entire recipe.

### 🛒 Smart Grocery Lists
Weekly grocery lists are sorted into categories (Proteins, Produce, Pantry, Dairy) with:
- **Buy-by date** — when to shop before the week starts
- **Day labels** — which night needs each ingredient
- **Tap to cross off** — check items as you shop
- **Share button** — native share sheet for texting to your shopper

### 📅 Meal Plans Tab
Save weekly plans to your account. View all saved weeks in the Meal Plans tab — tap any week to expand, tap any recipe to open the full recipe card with ingredients and steps.

### ⭐ Favorites & History
Star any recipe to save to Favorites. Full recipe history with search by name, style, or ingredient. Free plan shows last 5 recipes; paid plans get unlimited history.

### 🍽️ Dietary Preferences (21 options in 4 groups)

**Dietary Restrictions** — Vegan, Vegetarian, Pescatarian, No Pork, No Red Meat

**Allergens — Strict** — Gluten-Free, Dairy-Free, Nut-Free, Egg-Free, Shellfish-Free, Soy-Free

**Health Goals** — Low-Carb, Keto, High-Protein, Low-Sodium, Low-Calorie, Heart-Healthy, Anti-Inflammatory

**Lifestyle** — Paleo, Whole30, Mediterranean Diet

Allergens use strict "non-negotiable" language in the AI prompt. Health goals use flexible guidance language. Both are injected directly into every recipe generation request.

### 👨‍🍳 Personalized Chef
Name your AI chef during onboarding. The chef's name appears throughout the app and in every recipe generation prompt, creating a personal kitchen assistant feel.

### 📱 Progressive Web App
Full PWA — installable on iOS and Android home screens. Offline page, service worker, full icon set (16px–512px), splash screens.

---

## Tech Stack

| Layer | Service | Purpose |
|---|---|---|
| Frontend | GitHub Pages | All HTML/CSS/JS — `mealwheeliq.com` |
| Backend | Railway | Express.js API — `api.mealwheeliq.com` |
| Database | TiDB Cloud Serverless | All user data, MySQL-compatible |
| AI Recipes | Anthropic claude-sonnet-4-6 | Recipe generation + pantry photo scanning |
| Payments | Stripe (live mode) | Subscription billing + webhooks |
| Auth | JWT + bcrypt | Custom auth, 30-day tokens |
| PWA | Service Worker + Manifest | Installable, offline-capable |

---

## Pricing

| Feature | Free | Home Chef $4.99/mo | Family $9.99/mo |
|---|---|---|---|
| Tonight's Dinner spins | 5/month | Unlimited | Unlimited |
| Soup Creator | 5/month | Unlimited | Unlimited |
| Plan My Week | — | ✅ | ✅ |
| Weekly grocery list | — | ✅ | ✅ |
| Pantry photo scan | ✅ | ✅ | ✅ |
| Recipe history | Last 5 | Unlimited | Unlimited |
| Favorites | — | ✅ | ✅ |
| Meal Plans tab | — | ✅ | ✅ |
| Family profiles | — | — | Up to 4 |
| Blog access | ✅ | ✅ | ✅ |

---

## Blog & SEO

11 posts live at `mealwheeliq.com/blog/` with weekly publishing cadence:

- What to Make for Dinner Tonight
- How to Plan a Week of Family Dinners
- 5 Easy Weeknight Dinners Under 30 Minutes
- How to Build a Family Grocery List That Actually Works
- The Best Meal Planning Apps for Families in 2026
- Why We Stopped Doing Takeout
- The Organic Grocery Guide: What's Actually Worth It
- Meal Planning for Beginners: Start Here
- How to Reduce Food Waste with Smarter Meal Planning
- Feeding a Family of 4 on a Budget
- How to Meal Plan Around Your Family's Schedule *(latest)*

Every post includes Article + FAQPage JSON-LD schema for SEO and AEO (Answer Engine Optimization). Sitemap submitted to Google Search Console. One new post published weekly rotating through: Meal Planning, Quick Dinners, Grocery & Shopping, Healthy Eating, Family Life, Budget Cooking, Beginners, Smart Kitchen.

---

## Onboarding Flow

1. **Welcome** — app overview and feature preview
2. **Name your chef** — personalized AI chef name
3. **Allergies & restrictions** — 10-option grid, saved to dietary preferences
4. **Pantry scan** — photo of fridge/pantry, confirm/edit detected items, or type individual items
5. **First spin** — straight into Tonight's Dinner

---

## Deployment

**Frontend** → push to `main` branch → GitHub Pages auto-deploys in ~60 seconds

**Backend** → push to `main` branch in `mealswheel-api` repo → Railway auto-deploys in ~2 minutes
> ⚠️ "Wait for CI" must remain **disabled** in Railway settings — this repo has no GitHub Actions and the setting causes indefinite deployment hangs.

**Database** — TiDB Cloud Serverless, schema `mealwheeliq`. All tables auto-created on server boot via `createTables()`.

---

## Repository Structure

```
mealwheeliq/          ← this repo (GitHub Pages)
├── index.html        Landing page
├── login.html        Sign in / Sign up
├── app.html          Full authenticated app (3 modes)
├── blog/             SEO blog content (11 posts)
├── manifest.json     PWA manifest
├── sw.js             Service worker
├── sitemap.xml       Google Search Console sitemap
├── robots.txt        Crawler instructions
└── icons/            PWA icons (16px–512px)

mealswheel-api/       ← backend repo (Railway)
└── server.js         Express.js API (auth, recipes, DB, Stripe)
```

---

*Built by Bryan Michael Greer · MealWheelIQ · July 2026*
