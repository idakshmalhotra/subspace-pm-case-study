# Subspace.money - Complete Sitemap & Page Directory

## Quick Reference Tree

```
subspace.money/
├── / (Homepage)
├── /public-groups (Group Sharing)
├── /vendors (Vendor Dashboard)
├── /trending-subscriptions (Featured Subscriptions)
├── /mobile-recharge (Mobile Services)
├── /dth (TV Services)
├── /dth-plans (DTH Plans)
├── /electricity (Utilities)
├── /fastag (Toll Services)
├── /search (Search Page)
├── /blogs (Blog Hub - 256 posts)
│   ├── /blog/[slug-1]
│   ├── /blog/[slug-2]
│   └── ... /blog/[slug-256]
├── Footer Links (Limited Public Access)
│   ├── /privacy-policy [404]
│   ├── /terms-of-service [404]
│   ├── /refund-policy [404]
│   ├── /shipping-policy [404]
│   ├── /about [404]
│   └── /contact [404]
└── Mobile Apps
    ├── Google Play Store
    └── Apple App Store
```

## Accessible Pages (Verified)

### 1. Homepage: `/`
**Status:** ✅ Accessible  
**Type:** SPA Entry Point  
**Key Components:**
- Location selector with geolocation detection
- Address entry form (flat/building, floor, locality)
- Authentication interface (WhatsApp + Phone OTP)
- Featured brands section
- Shared subscriptions preview
- Bottom navigation (5 items)
- Footer with links

**Content:**
- Platform tagline: "Delivery in minutes"
- Address categories: Home, Work, Hotel, Other
- Verification code messaging

---

### 2. Blog Hub: `/blogs`
**Status:** ✅ Accessible  
**Type:** Content Hub  
**Features:**
- Category filtering (Cards offers, Discounts, OTT, Entertainment)
- Pagination support
- Article cards with thumbnails
- Publication dates
- Search within blogs

**Content Categories:**
- OTT/Streaming Services
- Financial Products & Services
- Payment APIs & Fraud Detection
- User Guides & Tutorials
- Discounts & Offers
- Company Announcements
- Business Subscriptions

**Article Count:** 256 posts spanning 2022-2026

---

### 3. Public Groups: `/public-groups`
**Status:** ✅ Accessible  
**Type:** Social Feature  
**Content:**
- Explanation of group sharing model
- 3-step process visualization:
  1. Join a group
  2. Share credentials
  3. Access premium at reduced cost
- Public groups listing
- "View All" navigation

---

## Service Pages (Limited Public Content)

| Page | URL | Status | Purpose |
|------|-----|--------|---------|
| Vendors | `/vendors` | ⚠️ Auth Required | Vendor management dashboard |
| Trending | `/trending-subscriptions` | ⚠️ Auth Required | Featured subscriptions |
| Mobile Recharge | `/mobile-recharge` | ⚠️ Auth Required | Phone plan recharge |
| DTH | `/dth` | ⚠️ Auth Required | TV subscription service |
| DTH Plans | `/dth-plans` | ⚠️ Auth Required | Available TV plans |
| Electricity | `/electricity` | ⚠️ Auth Required | Bill payment |
| FastTag | `/fastag` | ⚠️ Auth Required | Toll payment |
| Search | `/search` | ⚠️ Auth Required | Global search |

---

## Inaccessible Pages (404 Errors)

| Page | URL | Expected Content |
|------|-----|------------------|
| About Us | `/about` | Company mission, team, history |
| Contact | `/contact` | Support contact, form |
| Privacy Policy | `/privacy-policy` | Data privacy terms |
| Terms of Service | `/terms-of-service` | Legal terms |
| Refund Policy | `/refund-policy` | Refund procedures |
| Shipping Policy | `/shipping-policy` | Delivery terms |
| Blog Posts (256) | `/blog/[slug]` | Individual articles |

**Note:** These are listed in footer/sitemap but return 404. Likely served through:
1. Different URL patterns
2. API endpoints
3. Authentication gateways
4. JavaScript-rendered content

---

## Dynamic Content Areas

### Bottom Navigation (Always Present)
```
[Home] [Explore] [Wallet] [Chat] [Account]
```

### Footer Structure (Consistent)
```
Legal          Company        Social Media     Apps
├─ Privacy     ├─ About       ├─ LinkedIn      ├─ Google Play
├─ Terms       ├─ Contact     ├─ Instagram     └─ App Store
├─ Refund      └─ Blogs       ├─ Facebook
└─ Shipping                   └─ X (Twitter)
```

---

## Blog Post Categories & Topics

### OTT & Streaming (Primary Focus)
- Netflix subscription guides
- Prime Video plans
- Disney Hotstar offers
- YouTube Premium setup
- Apple TV content
- Streaming bundling strategies

### Financial Services
- UPI payment guides
- Credit card optimization
- Digital lending options
- Financial planning resources
- Investment tips

### Payments & APIs
- Superflow payment APIs
- Fraud detection systems
- Gift card platforms
- BBPS (Bill Payment System)
- Payment gateway integrations

### Utilities & Telecom
- Mobile recharge options
- DTH plan comparisons
- Electricity bill management
- FastTag setup guides

### Discounts & Promotions
- Gift card deals (AJIO, Amazon, Zomato)
- Coupon compilations
- Seasonal offers
- Platform discounts

### Business/Enterprise
- Subscription management software
- B2B SaaS solutions
- Enterprise billing
- Team collaboration tools

---

## URL Patterns

### Blog Posts
**Pattern:** `/blog/[descriptive-slug]`  
**Examples:**
- `/blog/what-is-subscription-management-software`
- `/blog/netflix-group-sharing-ban-create-a-family-plan`
- `/blog/[OTT/service-specific-guides]`

**Count:** 256 URLs  
**Date Range:** 2022 - May 2026

### Main Pages
**Pattern:** `/[service-name]`  
**Examples:**
- `/mobile-recharge`
- `/dth`
- `/electricity`
- `/fastag`

---

## Analytics & Performance Indicators

| Metric | Value |
|--------|-------|
| Total Sitemap Entries | 267 |
| Main Pages | 11 |
| Blog Articles | 256 |
| Navigation Items | 5 |
| Footer Link Groups | 4 |
| Address Categories | 4 |
| Service Categories | 8+ |
| Mobile Platforms | 2 |
| Social Networks | 4 |

---

## Page Access Requirements

### Public Access (No Auth)
- `/` (Homepage)
- `/blogs` (Blog listing)
- `/public-groups` (Overview)
- `/search` (Interface only)

### Authentication Required
- `/vendors`
- `/trending-subscriptions`
- `/mobile-recharge`
- `/dth`, `/dth-plans`
- `/electricity`
- `/fastag`
- `/wallet`
- `/explore`
- `/account`
- `/chat`

### Redirects/404
- Most footer links
- Individual blog posts
- Policy pages
- About/Contact pages

---

## Navigation Flow Map

```
Homepage (/)
    ↓
    ├─→ Explore [Trending Subscriptions, Vendors]
    ├─→ Wallet [Payment Management]
    ├─→ Chat [Support]
    ├─→ Account [Profile Settings]
    ├─→ Blogs [Content Hub]
    ├─→ Public Groups [Social Sharing]
    └─→ Services
        ├─ Mobile Recharge
        ├─ DTH
        ├─ Electricity
        └─ FastTag
```

---

## Technical Implications

### Frontend Stack
- Single Page Application (client-side routing)
- Dynamic content loading
- Address/location APIs
- Real-time chat integration
- Payment gateway integration

### Backend Requirements
- User authentication service
- Subscription database
- Vendor management system
- Payment processing
- Blog/CMS system
- Geolocation service
- Analytics service

### API Endpoints (Inferred)
- Auth endpoints (WhatsApp, OTP verification)
- Subscription CRUD operations
- Vendor APIs
- Payment/Wallet APIs
- Chat/Messaging APIs
- User profile APIs
- Location/Address APIs

---

## Recommendations for Testing/Analysis

1. **Authentication Flow Testing**
   - Create test accounts via WhatsApp
   - Test phone OTP verification
   - Analyze session management

2. **Service Navigation**
   - Test each service category (mobile, DTH, electricity, fastag)
   - Verify subscription listings
   - Check pricing and plans

3. **Group Sharing Flow**
   - Create/join groups
   - Test credential sharing
   - Verify cost calculations

4. **Payment Testing**
   - Add payment methods
   - Test transaction flow
   - Verify billing records

5. **Blog Content Analysis**
   - Extract all 256 blog posts
   - Categorize by topic
   - Analyze SEO strategy

---

*Last Updated: 2026-05-31*
*Total Discoverable Pages: 267 (11 public, 256 blog posts)*
