# ULTINO TOOL TECH - Wire-Cut EDM Job Card & Production Management System

A high-precision, production-grade Digital Job Card, Production Tracking, and Billing Ledger application designed for CNC & Wire-Cut EDM toolrooms and machine shops.

---

## 🚀 Key Features

1. **Digital Job Card Creation & Tracking**:
   - Auto-generated job numbers (`JOB 001`, `JOB 002`, ...).
   - Real-time Wire-Cut EDM calculation (Perimeter / Cut Length × Thickness = Area in mm² or sq-inch, Cutting Speed mm²/min, Total Machining Time, Cost Estimation).
   - Drawing attachments & technical sketches with canvas viewer.
   - Status tracking: *Production*, *Inspection*, *Ready for Dispatch*, *Dispatched*, *Billed*.

2. **🎙️ Voice Controller (Speech-to-Words Voice Recorder)**:
   - Real-time speech recognition (Speech-to-Text) streaming audio words directly into descriptions.
   - Live dynamic waveform audio visualizer (Web Audio API & Canvas).
   - Multi-language support (English, Hindi, Marathi, etc.).
   - Insert, Replace, Clear, and Dictate modes with dirty/oily hand convenience for workshop operators.
   - Floating Quick Voice Dictation button available anywhere in the app.

3. **Production Screen**:
   - Live machine floor timers with elapsed time tracking.
   - Quick one-click status transitions and operator notes.

4. **Monthly Ledger & Billing**:
   - Customer-wise billing summaries, payment status, PDF generation & export.

5. **Customer & Item Master Catalog**:
   - Reusable component specs, hourly/sq-mm cutting rates, and customer profiles.

6. **Offline-First & Data Backup**:
   - Fast client-side persistent storage via IndexedDB.
   - One-click full JSON backup export & restore.
   - Cross-device sync code transfer.

---

## 🛠️ Quick Start (Run Locally)

### Prerequisites
- Node.js (v18 or higher recommended)
- npm or pnpm or bun

### 1. Install Dependencies
```bash
npm install
```

### 2. Start the Development Server
```bash
npm run dev
```

Open your browser at:
`http://localhost:3000` or the port shown in your terminal.

### 3. Build for Production
```bash
npm run build
```

To preview the production build locally:
```bash
npm run preview
```

---

## 📁 Project Structure

```
├── index.html                  # HTML entry point
├── metadata.json               # App metadata
├── package.json                # Project dependencies and scripts
├── tsconfig.json               # TypeScript configuration
├── vite.config.ts              # Vite bundler configuration
├── public/                     # Static assets (logos, icons)
└── src/
    ├── main.tsx                # React root mount
    ├── App.tsx                 # Core application shell & navigation
    ├── types.ts                # TypeScript domain models
    ├── index.css               # Global Tailwind CSS styles
    ├── components/
    │   ├── Navbar.tsx          # Responsive navigation & mobile ergonomics
    │   ├── Dashboard.tsx       # Live status metrics & active jobs
    │   ├── JobCardForm.tsx     # Job creation & edit form with EDM calculator
    │   ├── ProductionScreen.tsx# Active machine floor monitoring
    │   ├── JobHistory.tsx      # Filterable & searchable job registry
    │   ├── CustomerMaster.tsx  # Customer CRM directory
    │   ├── ItemMaster.tsx      # Component & item master catalog
    │   ├── MonthlyLedger.tsx   # Billing ledger & PDF generator
    │   ├── BackupSettings.tsx  # IndexedDB export, import & sync
    │   ├── JobViewModal.tsx    # Detailed job inspector & print trigger
    │   ├── JobPrintView.tsx    # Formal printable Job Card layout
    │   ├── DrawingViewerModal.tsx # Fullscreen drawing inspector
    │   ├── VoiceDescriptionController.tsx # Voice recorder & Speech-to-Text
    │   └── FloatingVoiceModal.tsx # Quick floating voice assistant
    └── services/
        ├── storage.ts          # IndexedDB persistence layer
        └── exportService.ts    # PDF / CSV export utilities
```

---

© ULTINO TOOL TECH - Industrial Automation & Precision Engineering.
