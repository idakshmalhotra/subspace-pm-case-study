# Subspace.money - Key Product Flows & User Journeys

## Overview

This document maps out the critical user flows and product journeys through the Subspace.money platform, including subscription management, group sharing, utilities, and customer support.

---

## 1. NEW USER ONBOARDING FLOW

### Flow Diagram
```
START
  ↓
[Homepage Load]
  ↓
[Location Selector]
  ├─→ Auto-detect location?
  │   ├─ YES → Use geolocation
  │   └─ NO → Manual search/entry
  ↓
[Address Entry Form]
  ├─ Flat/Building number
  ├─ Floor
  ├─ Area/Locality
  ├─ Landmarks (optional)
  └─ Category selection (Home/Work/Hotel/Other)
  ↓
[Save Address]
  ↓
[Authentication Gate]
  ├─→ Login Method
  │   ├─ WhatsApp OAuth
  │   │   └─ Redirect to WhatsApp
  │   │   └─ Return with auth token
  │   └─ Phone Verification
  │       └─ Enter phone number
  │       └─ Receive OTP
  │       └─ Verify OTP
  ↓
[Create Account]
  ├─ Set up profile (optional)
  ├─ Payment method (optional)
  └─ Push notification consent (optional)
  ↓
[Welcome/Onboarding Tour]
  ├─ Platform overview
  ├─ Feature highlights
  └─ Suggested subscriptions
  ↓
[Dashboard/Home]
  ↓
END
```

### Key Steps
1. **Location Detection** → Geolocation or manual search
2. **Address Entry** → Complete delivery information
3. **Authentication** → WhatsApp or OTP verification
4. **Profile Creation** → Basic account setup
5. **Onboarding** → Platform orientation
6. **Dashboard Access** → Ready to browse/purchase

### Pain Points & Optimizations
- Address form could be pre-filled with geolocation data
- WhatsApp login reduces authentication friction
- Phone OTP provides non-social auth alternative
- Address categories (Home/Work) enable quick selection

---

## 2. SUBSCRIPTION DISCOVERY & PURCHASE FLOW

### Flow Diagram
```
[Dashboard/Home]
  ↓
[Browse Subscriptions]
  ├─→ Navigation Options:
  │   ├─ Explore tab
  │   ├─ Search functionality
  │   ├─ Featured/Trending
  │   ├─ Favorite Brands section
  │   └─ Categories (OTT, Finance, etc.)
  ↓
[Subscription Listings]
  ├─ View subscription cards
  ├─ See pricing & ratings
  ├─ Read reviews
  └─ Compare with alternatives
  ↓
[Select Subscription]
  ├─→ View Details Page
  │   ├─ Service description
  │   ├─ Plan options
  │   ├─ Pricing breakdown
  │   ├─ User reviews (rating, comments)
  │   ├─ Group sharing availability
  │   └─ FAQ
  ↓
[Select Plan/Option]
  ├─ Choose plan (if multiple)
  ├─ Select billing cycle (monthly/annual)
  ├─ Add any add-ons
  └─ Quantity selection (if applicable)
  ↓
[Add to Cart/Wallet]
  ├─ Item added notification
  └─ Continue shopping or proceed
  ↓
[Review Cart]
  ├─ Verify items
  ├─ See total cost
  ├─ Adjust quantities
  └─ Remove items
  ↓
[Proceed to Checkout]
  ↓
[Delivery Address Confirmation]
  ├─→ Select saved address
  │   ├─ Home
  │   ├─ Work
  │   └─ Other
  └─→ Or enter new address
  ↓
[Select Payment Method]
  ├─ Credit/Debit card
  ├─ Digital wallet
  ├─ UPI
  ├─ Net banking
  └─ Saved payment methods
  ↓
[Payment Processing]
  ├─ Verify payment details
  ├─ Process transaction
  ├─ Fraud checks
  └─ Payment confirmation
  ↓
[Order Confirmation]
  ├─ Order number
  ├─ Subscription details
  ├─ Expected activation
  ├─ Support contact
  └─ Option to add to calendar
  ↓
[Subscription Activation]
  ├─ Credentials sent (if applicable)
  ├─ Access granted
  ├─ Welcome email
  └─ First reminder (renewal date)
  ↓
[Dashboard Update]
  ├─ Subscription visible in "Active"
  ├─ Renewal date shown
  ├─ Credentials accessible (if shared)
  └─ Usage tracking enabled
  ↓
END
```

### Critical Decision Points
1. **Where to Browse?** → Navigation method affects discovery
2. **Which Plan?** → Price/features trade-off
3. **When to Pay?** → Immediate or scheduled
4. **Payment Method?** → Security & convenience
5. **Address Confirmation?** → For digital services, may not be needed

### Conversion Optimization
- **Reduce friction:** Pre-filled addresses, saved payment methods
- **Build trust:** Show reviews, ratings, user count
- **Create urgency:** Limited-time offers, group deals
- **Simplify:** One-click checkout, auto-renew options

---

## 3. GROUP SHARING & COST REDUCTION FLOW

### Flow Diagram
```
[Dashboard/Subscriptions]
  ↓
[Discover Group Sharing Feature]
  ├─ "Save more with shared subscriptions"
  ├─ "Join an existing group"
  └─ "Create a new group"
  ↓
[Option A: JOIN EXISTING GROUP]
  ├─ [Browse Public Groups]
  │   ├─ View available groups
  │   ├─ See member count
  │   ├─ Check cost per person
  │   ├─ Read group description
  │   └─ Sort/filter by service
  │
  ├─ [Select Group]
  │   ├─ View full details
  │   ├─ See members (anonymized)
  │   ├─ Understand cost split
  │   ├─ Check group rules
  │   └─ Review credentials usage
  │
  ├─ [Join Group]
  │   ├─ Accept terms
  │   ├─ Confirm cost
  │   ├─ Complete payment
  │   └─ Get added to group
  │
  ├─ [Receive Credentials]
  │   ├─ Secure credential sharing
  │   ├─ Encrypted password sharing
  │   ├─ 2FA setup (if available)
  │   └─ Test access
  │
  └─ [Active Membership]
      ├─ Access shared subscription
      ├─ See other members (optional)
      ├─ Manage your seat
      └─ Leave group option
  
  ↓
[Option B: CREATE NEW GROUP]
  ├─ [Select Subscription]
  │   └─ Choose which subscription to share
  │
  ├─ [Configure Group]
  │   ├─ Set max members
  │   ├─ Set member cost
  │   ├─ Add group description
  │   ├─ Set sharing rules
  │   └─ Privacy settings
  │
  ├─ [Invite Members]
  │   ├─ Generate invite link
  │   ├─ Share via WhatsApp/Email
  │   ├─ Manage pending invites
  │   └─ Auto-accept settings
  │
  ├─ [Credential Management]
  │   ├─ Upload credentials securely
  │   ├─ Set sharing method
  │   │   ├─ Show in-app
  │   │   ├─ Send via encrypted link
  │   │   └─ Manual share (external)
  │   ├─ Rotation schedule
  │   └─ Password change alerts
  │
  ├─ [Payment Collection]
  │   ├─ Auto-billing setup
  │   ├─ Manual payment requests
  │   ├─ Payment reminders
  │   └─ Payment tracking
  │
  └─ [Group Management]
      ├─ View all members
      ├─ Remove members
      ├─ Update rules
      ├─ Monitor activity
      └─ Manage disputes
  
  ↓
[Active Group Membership]
  ├─ Access subscription
  ├─ See cost savings
  ├─ Communicate with members
  ├─ Share feedback
  └─ Leave or manage seats
  ↓
END
```

### Cost Breakdown Example
```
Original Netflix Plan: ₹499/month
Group Size: 4 members
Cost per person: ₹499 ÷ 4 = ₹124.75 (~75% savings)

Payment Flow:
  Group Admin: ₹499 (pays full, covers all)
  OR
  Split Billing: Each member pays ₹125
  
Subspace Fee: ₹5-10 per member (for managing sharing)
```

### Group Sharing Benefits
- **Cost Savings:** 50-75% reduction per user
- **Convenience:** Automated credential sharing
- **Security:** Encrypted credential management
- **Community:** Meet like-minded users
- **Transparency:** Clear cost breakdown

### Risk Mitigation
- **Account Security:** Separate 2FA for each member
- **Terms Compliance:** Explain service ToS violations
- **Payment Disputes:** Automated collection & resolution
- **Member Removal:** Quick process for problematic users
- **Credential Rotation:** Regular password changes

---

## 4. UTILITY SERVICES FLOW

### 4A. Mobile Recharge Flow
```
[Dashboard] → [Services] → [Mobile Recharge]
  ↓
[Enter Phone Number]
  ├─ Mobile number input
  ├─ Auto-detect operator
  └─ Validate number
  ↓
[Select Plan]
  ├─ View available plans
  ├─ See validity period
  ├─ Check benefits
  └─ Compare prices
  ↓
[Confirm Details]
  ├─ Phone number: XXXXXXXXXX
  ├─ Operator: Jio/Airtel/Vodafone
  ├─ Plan: 28 days, 1.5 GB
  ├─ Price: ₹199
  └─ [Proceed to Payment]
  ↓
[Payment]
  ├─ Select method
  ├─ Complete transaction
  └─ Get confirmation
  ↓
[Activation]
  ├─ Plan activated immediately
  ├─ Confirmation SMS sent
  └─ Balance updated in app
  ↓
[Notification]
  ├─ Success notification
  ├─ Plan details
  └─ Next recharge reminder
  ↓
END
```

### 4B. DTH Subscription Flow
```
[Dashboard] → [Services] → [DTH]
  ↓
[Enter DTH Details]
  ├─ Subscriber number / Phone
  ├─ Select DTH operator (Dish, Tata Sky)
  └─ Validate account
  ↓
[View Current Plan]
  ├─ Current subscription
  ├─ Expiry date
  ├─ Channels included
  └─ Bill amount
  ↓
[Browse Plans]
  ├─ View all available plans
  ├─ See channel packages
  ├─ Compare prices
  └─ Check regional availability
  ↓
[Upgrade/Renew]
  ├─ Select new plan
  ├─ Add premium channels
  ├─ See prorated cost
  └─ Confirm change
  ↓
[Payment]
  ├─ Amount due
  ├─ Select payment method
  └─ Complete transaction
  ↓
[Confirmation]
  ├─ Plan updated
  ├─ New plan active immediately
  ├─ Confirmation SMS/Email
  └─ Channels updated
  ↓
END
```

### 4C. Electricity Bill Payment Flow
```
[Dashboard] → [Services] → [Electricity]
  ↓
[Select State/Utility]
  ├─ State selector
  ├─ Electricity board
  └─ Available distributors
  ↓
[Enter Consumer Details]
  ├─ Consumer number
  ├─ Phone number (verification)
  └─ Validate against DB
  ↓
[View Bill]
  ├─ Current bill amount
  ├─ Due date
  ├─ Previous bill history
  ├─ Usage details
  └─ Payment history
  ↓
[Select Payment Option]
  ├─ One-time payment
  ├─ Schedule recurring payment
  ├─ Pay partial amount
  └─ Set automatic payment
  ↓
[Payment Method]
  ├─ Credit/Debit card
  ├─ UPI
  ├─ Net banking
  └─ Digital wallet
  ↓
[Process Payment]
  ├─ Verify amount
  ├─ Complete transaction
  └─ Confirmation number
  ↓
[Confirmation]
  ├─ Payment successful
  ├─ Receipt available
  ├─ Utility notification sent
  ├─ Next payment reminder
  └─ Download bill copy
  ↓
END
```

### 4D. FastTag Flow
```
[Dashboard] → [Services] → [FastTag]
  ↓
[New User - Account Setup]
  ├─ Vehicle registration
  ├─ Vehicle type selection
  ├─ KYC verification
  └─ Bank account linking
  ↓
[Existing User - Account Access]
  ├─ View account balance
  ├─ Recent transactions
  ├─ Linked vehicles
  └─ Account status
  ↓
[Recharge FastTag]
  ├─ Current balance
  ├─ Select amount
  ├─ Payment method
  └─ Confirm recharge
  ↓
[Payment Processing]
  ├─ Deduct from wallet
  ├─ Auto-recharge (if set)
  └─ Confirmation
  ↓
[Transaction History]
  ├─ View toll deductions
  ├─ Location passed
  ├─ Time of passage
  └─ Amount deducted
  ↓
END
```

---

## 5. CUSTOMER SUPPORT & CHAT FLOW

### Flow Diagram
```
[Any Page/Issue Occurs]
  ↓
[Chat Icon/Tab]
  ├─ Floating chat button
  └─ Chat tab in navigation
  ↓
[Chat Interface Opens]
  ├─ Chat history visible
  ├─ Previous conversations
  └─ Quick reply options
  ↓
[Message Options]
  ├─ Type custom message
  ├─ Quick replies (preset)
  │   ├─ "Where's my order?"
  │   ├─ "How to join a group?"
  │   ├─ "Payment issue"
  │   ├─ "Refund request"
  │   └─ "Other"
  ├─ Attach document/screenshot
  └─ Send message
  ↓
[Message Queue]
  ├─ Message sent notification
  ├─ Timestamp recorded
  └─ Message stored
  ↓
[Support Agent Response]
  ├─ Bot/AI initial response
  │   └─ Quick answers
  ├─ OR Human agent takes over
  │   ├─ Agent assigned
  │   ├─ "Agent is typing..."
  │   └─ Real-time message
  ↓
[Resolution Options]
  ├─ Issue resolved
  │   ├─ Satisfaction rating
  │   ├─ Feedback form
  │   └─ Chat ends
  ├─ OR Escalation needed
  │   ├─ Transfer to specialist
  │   ├─ Create ticket
  │   └─ Follow-up schedule
  ↓
[Post-Support]
  ├─ Survey sent
  ├─ Rating & feedback
  ├─ Solution article sent
  └─ Chat archived
  ↓
END
```

### Common Support Issues & Resolutions
```
Category: Subscription Issues
  ├─ "Where's my subscription?"
  │   └─ Check order status, activation status
  ├─ "How to use credentials?"
  │   └─ Send access guide, credentials
  ├─ "Plan not activated"
  │   └─ Check payment, verify with provider
  └─ "Quality issue"
      └─ Troubleshoot, contact provider

Category: Payment Issues
  ├─ "Payment failed"
  │   └─ Check card/payment method
  ├─ "Duplicate charge"
  │   └─ Refund initiated
  ├─ "Refund not received"
  │   └─ Check refund status, escalate
  └─ "Payment declined"
      └─ Troubleshoot payment method

Category: Account Issues
  ├─ "Can't login"
  │   └─ Password reset, OTP resend
  ├─ "Account suspended"
  │   └─ Explain reason, appeal process
  ├─ "Missing subscription"
  │   └─ Recover, restore subscription
  └─ "Data privacy question"
      └─ Direct to privacy policy

Category: Group Sharing
  ├─ "How to join group?"
  │   └─ Step-by-step guide
  ├─ "Credentials not working"
  │   └─ Troubleshoot, request fresh creds
  ├─ "Member kicked me out"
  │   └─ Explain rules, offer alternatives
  └─ "Cost dispute"
      └─ Verify calculation, refund if needed
```

---

## 6. WALLET & PAYMENT MANAGEMENT FLOW

### Flow Diagram
```
[Dashboard] → [Wallet Tab]
  ↓
[Wallet Overview]
  ├─ Account balance
  ├─ Payment methods
  ├─ Transaction history
  └─ Upcoming payments
  ↓
[Add Payment Method]
  ├─ Select method type
  │   ├─ Credit card
  │   ├─ Debit card
  │   ├─ UPI
  │   ├─ Digital wallet
  │   └─ Net banking
  ├─ Enter details
  ├─ 3D Secure verification
  ├─ Save for future (optional)
  └─ Confirmation
  ↓
[Manage Payment Methods]
  ├─ View saved methods
  ├─ Set default payment
  ├─ Edit payment method
  ├─ Delete payment method
  └─ Verify for security
  ↓
[Load Wallet (Optional)]
  ├─ Add funds to wallet
  ├─ Select amount
  ├─ Choose payment method
  ├─ Complete payment
  └─ Funds credited
  ↓
[Transaction History]
  ├─ View all transactions
  ├─ Filter by type
  │   ├─ Purchases
  │   ├─ Refunds
  │   ├─ Transfers
  │   └─ Fees
  ├─ Download statements
  └─ Dispute transaction
  ↓
[Scheduled Payments]
  ├─ View upcoming bills
  ├─ Set auto-renew
  ├─ Adjust payment date
  ├─ Auto-update payment method
  └─ Cancel recurring
  ↓
[Refunds & Disputes]
  ├─ View refund status
  ├─ Track refund timeline
  ├─ Dispute charge
  └─ Escalate issue
  ↓
END
```

---

## 7. ACCOUNT SETTINGS & PROFILE FLOW

### Flow Diagram
```
[Dashboard] → [Account Tab]
  ↓
[Account Settings Main]
  ├─ [Profile Information]
  │   ├─ Name/Username
  │   ├─ Email
  │   ├─ Phone number
  │   ├─ Profile picture
  │   └─ Bio/About
  │
  ├─ [Address Management]
  │   ├─ View saved addresses
  │   ├─ Add new address
  │   ├─ Edit existing
  │   ├─ Delete address
  │   └─ Set as default
  │
  ├─ [Privacy & Security]
  │   ├─ Password change
  │   ├─ 2FA setup
  │   ├─ Connected devices
  │   ├─ Login history
  │   ├─ Blocked users
  │   └─ Data export
  │
  ├─ [Notification Preferences]
  │   ├─ Email notifications
  │   ├─ SMS notifications
  │   ├─ Push notifications
  │   ├─ Notification frequency
  │   └─ Opt-out options
  │
  ├─ [Preferences]
  │   ├─ Language selection
  │   ├─ Currency
  │   ├─ Theme (light/dark)
  │   └─ Default categories
  │
  ├─ [Subscription Management]
  │   ├─ View active subscriptions
  │   ├─ Pause subscription
  │   ├─ Cancel subscription
  │   ├─ Change payment method
  │   └─ Renewal reminders
  │
  ├─ [Group Memberships]
  │   ├─ View joined groups
  │   ├─ Leave group
  │   ├─ Manage group roles
  │   └─ Invite status
  │
  ├─ [Support & Legal]
  │   ├─ Contact support
  │   ├─ Privacy policy
  │   ├─ Terms of service
  │   ├─ Refund policy
  │   ├─ Shipping policy
  │   ├─ Cookie policy
  │   └─ Community guidelines
  │
  ├─ [Account Actions]
  │   ├─ Download data
  │   ├─ Close account
  │   └─ Report abuse
  │
  └─ [Logout]
      └─ Sign out of account
  ↓
END
```

---

## 8. BROWSE & SEARCH FLOW

### Flow Diagram
```
[Dashboard/Home]
  ↓
[Choose Discovery Method]
  ├─→ [Browse by Category]
  │   ├─ OTT/Streaming
  │   ├─ Finance/Banking
  │   ├─ Utilities
  │   ├─ Telecom
  │   ├─ Gaming
  │   ├─ Productivity
  │   └─ Other
  │
  ├─→ [Trending/Featured]
  │   ├─ Most popular this week
  │   ├─ Newly added
  │   ├─ Editor's picks
  │   └─ Exclusive deals
  │
  ├─→ [Search]
  │   ├─ Search bar
  │   ├─ Voice search (optional)
  │   ├─ Recent searches
  │   └─ Search suggestions
  │
  └─→ [Favorite Brands]
      ├─ Pre-selected brands
      ├─ Add to favorites
      └─ One-click access
  ↓
[View Results/Listings]
  ├─ Subscription cards
  ├─ Sorting options
  │   ├─ Price (low-high)
  │   ├─ Rating (best first)
  │   ├─ Newest
  │   ├─ Most popular
  │   └─ Savings potential
  ├─ Filtering options
  │   ├─ Price range
  │   ├─ Rating
  │   ├─ Group available
  │   ├─ Trial available
  │   └─ Provider
  └─ Pagination/Infinite scroll
  ↓
[Subscription Details View]
  ├─ Service name & logo
  ├─ Description
  ├─ Rating & reviews
  ├─ Pricing & plans
  ├─ Group sharing info
  ├─ Provider details
  ├─ FAQs
  └─ [Subscribe]
  ↓
END
```

---

## 9. BLOG & CONTENT CONSUMPTION FLOW

### Flow Diagram
```
[Dashboard] → [Blogs Link / Blog Page]
  ↓
[Blog Hub]
  ├─ Featured articles
  ├─ Category filter
  └─ Search articles
  ↓
[Browse Articles]
  ├─ View article cards
  ├─ See thumbnails
  ├─ Read summaries
  ├─ Check publication date
  ├─ Sort by recent/popular
  └─ Pagination
  ↓
[Read Article]
  ├─ Full article view
  ├─ Comments/discussion
  ├─ Share options
  ├─ Related articles
  ├─ Author info
  └─ Reading time estimate
  ↓
[Engagement Options]
  ├─ Like/Upvote article
  ├─ Share on social
  ├─ Comment/discuss
  ├─ Save for later
  ├─ Newsletter signup
  └─ Related article links
  ↓
[Content Discovery]
  ├─ Related articles
  ├─ Category deep dive
  ├─ Author's other posts
  └─ Trending topics
  ↓
END
```

---

## Key Metrics & Tracking

### Purchase Flow Conversion
```
Visitors → Users → Authenticated → Browsing → Added to Cart → Checkout → Paid
100%    → 40%   → 35%            → 30%      → 15%          → 10%       → 8%

Target: Improve each conversion rate by 20%
Critical drop-off: Add to cart → Checkout
```

### Group Sharing Adoption
```
Viewing groups → Joining → Active members → Cost savings realized
100%           → 30%     → 85%            → 92%
```

### Customer Satisfaction
```
Target NPS: > 50
Target CSAT: > 85%
Support resolution time: < 4 hours
```

---

## Future Enhancement Opportunities

1. **AI-Powered Recommendations:** Smart suggestions based on usage
2. **Subscription Analytics:** Spending insights and optimization tips
3. **Family Plans:** Dedicated family sharing with parental controls
4. **Loyalty Program:** Rewards for group creation and referrals
5. **Subscription Prediction:** ML-based renewal reminders
6. **API Integration:** Direct provider integrations for auto-top-up
7. **Voice Search:** "Hey Subspace, recharge my mobile"
8. **AR Features:** Visual plan comparison
9. **Social Features:** Connect with friends, share wishlists
10. **Blockchain Verification:** Credential authenticity verification

---

*End of Product Flows Document*  
*Last Updated: 2026-05-31*
