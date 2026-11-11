# Iron & Lime — Gym Management System

> **"Run the floor. Not the spreadsheets."**  
> A comprehensive, modern gym management platform built with high performance, role-based security, and an ergonomic staff interface.

---

## 🏋️ Overview

**Iron & Lime** is a single-system console designed for gym owners, managers, reception staff, and trainers. It replaces fragmented spreadsheets and disjointed tools with a unified operations dashboard, real-time check-in kiosk, recurring billing tracker, and fitness schedule engine.

---

## 🚀 Key Features

### 1. 📊 Executive Dashboard
- **Live Floor Analytics**: Real-time counter of checked-in members on the gym floor.
- **Financial Pulse**: Month-to-date collected revenue vs. pending invoices.
- **Staff & Schedule Overview**: Active trainers on duty, active memberships in good standing, and weekly class rosters.
- **Revenue Trend & Attendance Charts**: Interactive Chart.js visual analytics.

### 2. 👥 Member Management (`members.html`)
- Complete member lifecycle tracking (Active, Inactive, Suspended).
- Membership plan assignment, emergency contact info, and medical flags.
- Instant search, status filtering, and quick member profile viewing.

### 3. 💳 Membership Plans (`memberships.html`)
- Tiered membership configuration (Basic, Premium, VIP All-Access, Student, Day Pass).
- Flexible billing intervals (Monthly, Quarterly, Annually, Pay-Per-Visit).
- Active subscriber counts and automated renewal calculations.

### 4. ⏱️ Check-In & Floor Attendance (`attendance.html`)
- 1-click member check-in and checkout.
- Real-time time-stamp logs with duration tracking.
- Visual status badges to confirm active membership validity before entry.

### 5. 🗓️ Class Scheduling & Bookings (`classes.html`)
- Dynamic weekly timetable for fitness sessions (HIIT, Spin, Yoga, Strength, Boxing).
- Trainer assignments, room locations, and capacity thresholds.
- Member booking list and capacity overflow prevention.

### 6. 🧑‍🏫 Trainer Profiles & Rosters (`trainers.html`)
- Trainer specialties, contact details, assigned classes, and active trainees.
- Performance statistics and schedule management.

### 7. 💰 Billing, Invoices & Payments (`payments.html`)
- Automated invoice generator with line items.
- Status tracking: Paid, Pending, Overdue.
- Multi-method transaction logging (Credit/Debit Card, Bank Transfer, Cash).

### 8. 🛠️ Equipment Maintenance Tracker (`equipment.html`)
- Gym asset registry (Treadmills, Power Racks, Cables, Dumbbells).
- Service history, maintenance warranty warnings, and breakdown reporting.

### 9. 🥗 Nutrition & Workout Plans (`nutrition.html`, `workouts.html`)
- Personalized diet plans and caloric guidelines.
- Workout routine templates tailored for strength, hypertrophy, or fat loss.

### 10. 📢 Announcements & System Reports (`announcements.html`, `reports.html`)
- Broadcast gym-wide notices to staff and members.
- Exportable CSV/PDF operational reports and financial audits.

---

## 🔐 Role-Based Access Control (RBAC)

The system includes preconfigured demo accounts for testing different permission tiers:

| Role | Username | Password | Access Level |
| :--- | :--- | :--- | :--- |
| **Admin** | `admin` | `admin123` | Full access across all modules, settings, financials, and staff management |
| **Receptionist** | `reception` | `front123` | Front-desk operations: Member lookup, check-ins, payments, and class attendance |
| **Trainer** | `trainer` | `train123` | Class timetables, assigned members, workout regimens, and nutrition plans |

---

## 🎨 Design System & Palette

The user interface uses a high-contrast athletic theme built on clean typography:

- **Primary Deep Teal**: `#0E2B27` (Sidebar & Hero dark areas)
- **Signature Lime**: `#CFFF3D` (Action buttons, active nav indicators, key badges)
- **Oat/Sage Canvas**: `#F5F7F5` (Comfortable eye-strain-free background)
- **Crisp Panels**: `#FFFFFF` with `#DCE3DF` subtle borders
- **Typography**: `Barlow Condensed` for bold athletic headlines and `Inter` for clean data readability

---

## 💻 Tech Stack

- **Frontend**: Modern Semantic HTML5, Vanilla JavaScript (ESModules), Tailwind CSS, Chart.js
- **Server / Bundler**: Vite (Fast HMR & build optimization), Express runtime proxy
- **Compatibility**: Mobile responsive drawer navigation + dedicated smartphone bottom-tab navigation bar for handheld floor tablets and phones

---

## 🛠️ Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- npm or bun

### Installation & Run

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start the local development server**:
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your web browser.

3. **Build for production**:
   ```bash
   npm run build
   ```

---

## 📁 Directory Structure

```text
├── index.html            # Split-screen brand hero & staff authentication
├── dashboard.html        # Main gym operations overview & analytics
├── members.html          # Member directory & profile management
├── memberships.html      # Subscription plans & pricing tiers
├── attendance.html       # Front-desk check-in kiosk & floor logs
├── classes.html          # Fitness class timetable & bookings
├── trainers.html         # Personal trainers & coaching staff
├── payments.html         # Invoices, billing cycles & receipts
├── equipment.html        # Equipment inventory & maintenance log
├── workouts.html         # Custom workout routine builder
├── nutrition.html        # Diet & meal plan tracker
├── reports.html          # Financial, attendance & retention reports
├── announcements.html    # Notice board & staff broadcasts
├── settings.html         # Gym configuration & system preferences
├── profile.html          # User profile & account security
├── css/
│   └── style.css         # Iron & Lime design system & custom components
└── js/
    └── common.js         # Core Auth engine, RBAC, modal handlers & data store
```

---

## 📄 License
Internal Staff Gym Management System © 2026 Iron & Lime Fitness. All rights reserved.
