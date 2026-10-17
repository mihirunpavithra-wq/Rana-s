# 📸 Rana's Story — Photography Portfolio & Real-time Booking Website

A modern, high-performance photography portfolio and automated booking web application for **Rana's Story**.

---

## ✨ Features Built Exactly to Your Request

1. **Photographer Details & Story (`src/components/About.jsx`)**:
   - Meet Rana: Photography philosophy, experience counters (300+ Weddings, 7+ Years Experience, 500+ Happy Couples).
   - Professional Gear details & quality assurance.

2. **Previous Work Showcase / Portfolio (`src/components/Portfolio.jsx`)**:
   - Filterable gallery categories: **Weddings**, **Pre-Shoots & Couples**, **Portraits**, and **Events**.
   - Full-screen interactive **Lightbox Modal** with high-resolution image viewing, captions, shoot venues, and quick inquiry buttons.

3. **Client Date Selection & Direct WhatsApp Booking (`src/components/BookingCalendar.jsx`)**:
   - Interactive calendar showing upcoming months.
   - Available dates are clearly marked in green/neutral and clickable.
   - Selecting a date automatically fills the **WhatsApp Booking Form**.
   - Client enters their name, phone, package, event type, and notes.
   - One-click **"Confirm & Book via WhatsApp"** button opens WhatsApp with a pre-formatted message:
     ```text
     📸 *NEW BOOKING INQUIRY - RANA'S STORY* 📸
     ------------------------------------
     Hello Rana, I would love to check and book your photography services!

     📅 *Requested Date:* 2026-11-28
     🎉 *Event / Shoot Type:* Wedding Photography
     💎 *Selected Package:* Signature Wedding Story
     📍 *Shoot Location / Venue:* Shangri-La Colombo
     👤 *Client Name:* Kasun & Sanduni
     📱 *Client Phone:* 077 123 4567
     ------------------------------------
     ```

4. **Google Calendar Live Sync (Automated "BOOKED" status)**:
   - When you record a booking in your Google Calendar (from your phone or PC), the website automatically reads it and marks that date with a **🔒 BOOKED** red badge.
   - Booked dates cannot be double-booked by other clients!
   - Built-in **Google Calendar Settings Modal** & **Admin Mode** (allows toggling dates directly or syncing with a public Google Calendar iCal link).

---

## 🚀 How to Run Locally

```bash
cd C:\Users\mathe\.gemini\antigravity\scratch\ranas-story
npm run dev
```
Open **http://localhost:5173** in your web browser.

---

## ⚙️ How to Connect Your Google Calendar

1. Open [Google Calendar](https://calendar.google.com) on your computer.
2. In the left panel, find the calendar where you keep your photography bookings.
3. Click the **3 dots** next to the calendar name &gt; **Settings and sharing**.
4. Under **"Access permissions for events"**, check the box **"Make available to public"** (You can select *"See only free/busy"* or *"See all event details"*).
5. Scroll down to the **"Integrate calendar"** section and copy the **"Public address in iCal format"** (ends with `.ics`).
6. On your website, click the **"Google Calendar Settings"** button and paste your link!

---

## 📱 How to Customize Your Phone & Social Links

Edit `src/data/portfolioData.js`:
- `whatsappNumber`: Your WhatsApp number in international format without `+` (e.g. `94771234567`).
- `phoneDisplay`: Display format (e.g. `+94 77 123 4567`).
- `email`: Your business email.
- `portfolioItems`: Add your own photos, couples' names, and wedding venues!
- `packages`: Modify prices and package deliverables.
