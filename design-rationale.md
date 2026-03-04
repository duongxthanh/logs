# Design Rationale — Waterfront Village Website

## 1. What's new in the design?

The new Waterfront Village website is completely redesigned with **7 main sections**, replacing the old structure (5 long scrolling, heavy-text sections). Below is the detail of each section and the design rationale.

---

### 1.1 Fullscreen Teaser Video (Hero Section)

**Changes:** Replaced the static image with a fullscreen teaser video, Waterfront Village logo placed on top.

**Why:**
- Video conveys the atmosphere, sound, and scale of Waterfront Village much more effectively than a static image — *especially important* because this is an entertainment-heavy venue (water show, stage show, fire dance).
- Creates a strong immediate impression when visitors land on the page.
- Logo on top of the video ensures brand presence from the very first second.

**Current state:** Video autoplays, loops continuously, muted (so as not to disrupt the browsing experience).

---

### 1.2 Interactive Sitemap

**Changes:** Added a comprehensive map of the entire Waterfront Village with **14 interactive points**, supporting fullscreen zoom.

**Why:**
- Waterfront Village has **14 venues** spread across a massive complex — customers need to understand the overall layout before diving into each specific venue.
- The map is placed right after the video, acting as a **"journey map"** to help customers orient themselves before scrolling further.
- Visitors can hover (on PC) or tap (on mobile) on each point to view a quick summary: name, description, area, capacity.

**Features:**
- **14 points** are marked accurately on the map with small colored circles, not obstructing the venue logos.
- **Fullscreen mode:** Customers can expand the map, zoom in/out, and drag to view details.

---

### 1.3 Restaurants & Bars (Dining Tabs)

**Changes:** Consolidated all restaurants and bars/cafés into a **single section** with 2 toggle tabs, instead of listing them one by one.

**Why:**
- The old version listed 7 dining venues vertically → the page was too long, making customers lose patience before reaching the end.
- The tab layout significantly reduces page length, neatly organizing the content.
- Clear categorization: **"Restaurants"** (3 venues: RockSalt, Spice Kitchen, Morning Glory) vs **"Bars & Cafés"** (4 venues: Heaven & Earth, The Workshop, Life Café, Moon Tower).
- Smooth tab transitions create a professional feel.

**Each venue card displays:**
- Ambience image + logo overlay at the bottom corner.
- Short description, key highlights, seating capacity.
- A **"Learn More"** button for each venue.

---

### 1.4 & 1.5 Entertainment — Village Water Show & The Stage

**Changes:** Separated entertainment into **2 distinct sections**, each with an alternating layout (image/video on the left, content on the right, and vice versa):
1. **Village Water Show** — real-life video + key highlights
2. **The Stage Dining & Show** — real-life video + key highlights

**Why:**
- The old version described entertainment in a long paragraph → hard to skim, causing customers to miss important info.
- **Bullet points** replace long paragraphs — each bullet is a clear highlight (fire dance, water puppets, seafood buffet...).
- **Real-life videos** replace static images — allowing customers to feel the live performance atmosphere.
- **Alternating layout** (video left/right) creates rhythm while scrolling, preventing boredom.

**"Booking Now" button:**
When clicked, a **booking form** appears directly on the page (popup). Customers can fill in their reservation details: date, time, number of guests, preferred venue, name, phone number, and submit directly — **no need to leave the page or make a phone call**.

---

### 1.6 Private Events

**Changes:** A dedicated section for private events, using a similar layout but with a **"Contact Us"** button instead of "Booking Now".

**Why:**
- Private events require a tailored process (direct consultation, not a simple online booking).
- Bullet points emphasize top advantages: 10 spaces, 500-guest capacity, full-service event organization.
- Kept separate from entertainment to clearly distinguish: *watching a show* (book tickets) vs *hosting an event* (contact for consultation).

**"Contact Us" button:**
When clicked, the phone automatically **calls the Waterfront hotline (+84 81 328 7226)** for direct consultation. On desktop, the browser asks to open the associated calling app.

---

### 1.7 Footer — Contact Info & Map

**Changes:** A brand new footer designed specifically for Waterfront (no longer using the generic Taste Vietnam footer).

**Why:**
- The old footer had a broken Google Map (didn't load) and a generic design that didn't fit the Waterfront tone.
- The new footer uses a dark background with gold accents — matching the luxurious aesthetic.
- Information is split into 3 separate, easy-to-read boxes:
  - **Opening Hours**
  - **Address**
  - **Get in Touch**: Phone, email, TripAdvisor
- Google Map displays the exact Waterfront Village location with the appropriate zoom level.

---

## Overall Page Structure

```text
┌─────────────────────────────────────────┐
│ 1. Fullscreen Teaser Video              │  ← First Impression
├─────────────────────────────────────────┤
│ 2. Interactive Sitemap                  │  ← Overview & Orientation
├─────────────────────────────────────────┤
│ 3. Restaurants & Bars (2 tabs)          │  ← Restaurants + Bars & Cafés
│    ┌───────────────┬───────────────┐    │
│    │ Restaurants   │ Bars & Cafés  │    │
│    └───────────────┴───────────────┘    │
├─────────────────────────────────────────┤
│ 4. Village Water Show                   │  ← Video + Highlights + Booking
├─────────────────────────────────────────┤
│ 5. The Stage Dining & Show              │  ← Video + Highlights + Booking
├─────────────────────────────────────────┤
│ 6. Private Events                       │  ← Image + Highlights + Contact
├─────────────────────────────────────────┤
│ 7. Footer — Contact Info & Map          │  ← Opening Hours + Address + Map
└─────────────────────────────────────────┘
```

### Core Design Principles

| Principle | Execution |
|---|---|
| **Visuals First** | Video/images take up ≥50% of each section; text is minimized, using bullet points |
| **Reduce Scrolling** | Tabs for dining; overview map instead of endless lists |
| **Clear Call to Actions** | Every section has an action button: Explore (map), Learn More (dining), Booking Now (shows), Contact Us (events) |
| **Luxurious Tone** | Serif fonts, uppercase headers, gold accents, ample whitespace |
| **Cross-Device Compatibility** | Responsive — displays perfectly on mobile, tablet, and desktop |

---

## 2. Which requirements have been met?

| # | Requirement | Status | Notes |
|---|-------------|--------|-------|
| 1 | **"There should be some tabs/home/About etc"** — Need tabs/navigation | ✅ Met | Two tabs for Dining (Restaurants / Bars & Cafés). Page is neatly divided into 7 flowing sections: Video → Map → Dining → Shows → Events → Footer |
| 2 | **"This looks for mobile phone only"** — Old version was mobile-only | ✅ Met | The design works flawlessly on both desktop (2 columns, horizontal layout) and mobile (1 column, vertical stack). Interactive map supports zoom on both |
| 3 | **Divide Waterfront into 3 categories:** Entertainment, Dining, Private Events | ✅ Met | Exactly 3 groups: Dining (Section 3), Entertainment (Sections 4+5), Private Events (Section 6) |
| 4 | **Entertainment = Indoor Theatre + Outdoor Cultural Show** | ✅ Met | Two separate sections: "Village Water Show" (outdoor) + "The Stage Dining & Show" (indoor) |
| 5 | **"Not too much text more pictures and videos"** | ✅ Met | Bullet points replace long paragraphs. Videos used for Hero + 2 shows. Ambient images for dining venues |
| 6 | **Put brochure info (logo, description, highlights, seats) on website** | ✅ Met | 7 venue cards display everything: logo, ambient image, description, highlights, seats |
| 7 | **Properly group restaurants and bars** (per old mockup) | ✅ Met | Restaurants (3): RockSalt, Spice Kitchen, Morning Glory. Bars & Cafés (4): Heaven & Earth, The Workshop, Life Café, Moon Tower |
| 8 | **Properly separate the 2 shows** (per old mockup) | ✅ Met | Water Show + The Stage are split into 2 sections with alternating layouts |

---

## 3. Items Pending Confirmation & Optimization

### 3.1 Old Images/Video — Needs Replacement

All current images are **old placeholders** that do not reflect the actual atmosphere of each venue. Specifically, only **3 images** are being reused across **9 locations** — none of which are the actual photos of their corresponding venues.

| Venue | Currently Displaying | To Be Replaced With |
|-------|----------------------|---------------------|
| Hero Section | Logo overlay | ✅ Keep or swap for new logo if available |
| RockSalt Steakhouse | Generic image (gallery_2) | 🔴 Actual RockSalt interior photo |
| Spice Kitchen | Generic image (booking_1) | 🔴 Actual Spice Kitchen interior photo |
| Morning Glory Seafood | Generic image (wedding) | 🔴 Actual Morning Glory interior photo |
| Heaven & Earth | Generic image (gallery_2) — duplicate of RockSalt | 🔴 Actual Heaven & Earth Lounge photo |
| The Workshop | Generic image (booking_1) — duplicate of Spice Kitchen | 🔴 Actual The Workshop photo |
| Life Café | Generic image (wedding) — duplicate of Morning Glory | 🔴 Actual Life Café photo |
| Moon Tower | Generic image (gallery_2) — duplicate of RockSalt | 🔴 Actual Moon Tower photo |
| Private Events | Generic image (wedding) — duplicate of Morning Glory | 🔴 Actual private event/banquet photo |

> **Summary:** We need **9 new, venue-specific photos** from the photography or marketing team.

### 3.2 "Learn More" buttons — Detail pages missing

Currently, every venue card in the Dining section has a **"Learn More"** button, but clicking it **leads nowhere** because we don't yet have dedicated detail pages for each restaurant/bar.

**Action Required:**
- Provide detailed content for each restaurant/bar so we can build individual detail pages.
- Or, hide the "Learn More" button until we are ready to implement them.

### 3.3 Missing Social Media Links

The Footer currently only has a **TripAdvisor** link. Waterfront Village needs to add other social media channels:

| Channel | Status | Action |
|---------|--------|--------|
| TripAdvisor | ✅ Available | — |
| Facebook Fanpage | ❌ Missing | Provide Fanpage link to add to Footer |
| YouTube Channel | ❌ Missing | Provide YouTube link (if any) to add to Footer |
| Instagram | ❌ Missing | Provide Instagram link (if any) to add to Footer |
| Zalo OA | ❌ Missing | Provide Zalo Official Account link (if any) |

### 3.4 'The Workshop' location undefined on sitemap

The Workshop needs to be integrated into the sitemap layout.
