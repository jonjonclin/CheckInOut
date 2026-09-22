# Student & Tutor Check-In & Check-Out Kiosk System

**https://github.com/jonjonclin/CheckInOut/releases** [link](https://github.com/jonjonclin/CheckInOut/releases)

A simple, fast, and free Check-In/Check-Out system designed for students and tutors. It runs smoothly on legacy hardware (Windows, macOS) with a minimal memory footprint (~40–50 MB RAM).

| Type | Link |
| :--- | :--- |
| **Venmo** | [Donate via Venmo App](venmo://paycharge?txn=pay&recipients=Jonathan-Lin-630) (@Jonathan-Lin-630) |

<p align="left">
  <img src="./qr_Jonathan_venmo.png" alt="Venmo QR Code" width="180" height="180" />
</p>

Support the project on Venmo: **@Jonathan-Lin-630**

---

## 🌟 Key Features

### 1. Front-End Kiosk View
* **Barcode & QR Code Scanner (Zero-Click Check-In/Out)**: Seamlessly supports any standard USB or Bluetooth 1D/2D barcode or QR code scanner (HID Keyboard Wedge). Students and tutors can simply scan their badge card for instantaneous check-in or check-out with audio chime and visual confirmation.
* **Visual Gallery Selection**: Students and tutors can tap/click their name card directly from a visual gallery or use the search bar/role filter (`All Users`, `🎓 Students`, `👨‍🏫 Tutors`).
* **Dual PIN Input (Touch Keypad & Keyboard)**: Enter PIN using either the touch on-screen numeric keypad or physical keyboard (top-row numbers, numpad, `Backspace` to edit, `Enter` to confirm, and `Escape` to cancel).
* **Instant Confirmation**: Audio/visual feedback banners confirm check-in and check-out status and calculate total session time.

### 2. Lock Screen / Kiosk Saver
* **Password-Protected Fullscreen Kiosk Mode**: Intercepts shortcut keys (`Alt+F4`, `Esc`, `Win key`, `Ctrl+W`) and locks the screen into fullscreen mode.
* **Manager Passcode Protection**: Prevents kids or unauthorized users from closing the app or navigating away without entering the Manager Password (default: `admin123`).

### 3. Manager Admin Dashboard
* **User Management (CRUD & Lifecycle)**:
  * Add, edit, remove, or reset PINs for students and tutors.
  * **🟢 Active vs ⏸️ Inactive Status Lifecycle**:
    * Set users as **Active** (visible on Kiosk for daily check-in/out) or **Inactive** (temporarily paused, graduated, or seasonal students).
    * **Attendance History Permanently Preserved**: Deactivating a student leaves all historical logs, timestamps, hours, and past reports completely intact.
    * **Check-In Blocking**: Inactive students cannot accidentally check in or out via kiosk tap or barcode scan.
    * **Roster Status Filtering**: Quickly toggle between `Active Only` (default), `Inactive Only`, or `All Status` across Desktop and Web portals.
    * **Safe Deletion Warning**: The system warns administrators that deleting permanently erases logs and recommends deactivating instead.
* **Student Attendance History & Individual Export**:
  * Double-click any student or click **"📋 Attendance History"** to inspect total sessions attended, total hours logged, and complete chronological check-in/out records.
  * 1-click individual student CSV export for parent inquiries and student time auditing.
* **Full User Roster CSV Export**:
  * Export all active and inactive students and tutors to a standardized CSV file (`User ID`, `Full Name`, `Role`, `Age`, `Check-In Code`, `Account Status`, `Kiosk Activity`, `Created At`).
* **Interactive Column Sorting & Multi-Selection**:
  * Clickable column headers (ID, Full Name, Role, Age, PIN, Status) with bidirectional sort indicators (▲/▼) in both Desktop (`ttk.Treeview`) and Web (`data-table`).
  * Checkboxes (Web) and multi-row selection (Desktop) for bulk actions.
* **Printable ID Badges & Address Labels**: 1-click generation of formatted, printable student and tutor badge sheets (`badges.html`).
  * **Target User Selection (New or Old / Active or Inactive)**: Highlight specific students/tutors directly in the roster table to print badges for just those individuals, or click the **🖨️ Badge** button on any user row for instant 1-click single-student printing.
  * **Standard Avery 5160 (30-up Address Labels) [Default]**: Pre-configured to print 30 labels per letter size sheet (1" × 2⅝") for easy, affordable peel-and-stick ID badges.
  * **Additional Formats**:
    * 🏷️ **10-shipping**: Shipping / Large Badge (10 / sheet • 2" × 4" Avery 5163)
    * 💳 **10-card**: ID Card / Clip Badge (10 / sheet • 2" × 3.5" Avery 5371)
    * 🪪 **8-card**: Cardstock Pass (8 / sheet • 2¼" × 3¾" Avery 5395)
  * **No Student Age on Badges**: Student age is completely omitted from printing for privacy and a clean, uncluttered look.
  * **1D Linear Barcode (Code 128)**: Crisp vector SVG barcodes designed for instant scanning with standard handheld USB/Bluetooth barcode scanner guns.
  * **2D Matrix Code (QR Code)**: High-contrast QR codes for smartphone/tablet camera scanners and 2D imagers.
  * **Both (Hybrid Format)**: Dual 1D + 2D codes on each badge card for universal scanner compatibility.
  * **In-Browser Format & Size Switcher**: Interactive toolbar buttons in `badges.html` to preview, switch sheet sizes, and toggle barcode formats right before printing.
  * **Safe Path Protection**: Automatically resolves to `~/Downloads` without root or system directory permission errors on macOS and Windows.
* **Bulk CSV Import**: Import student/tutor records from any custom `.csv` file with interactive **Field Mapping** (maps Full Name, Role, Age, and PIN Code columns, with automatic 4-digit PIN generation for missing codes).
* **Attendance & Duration Reports**:
  * **Quick Date Range Presets**: 1-click presets (`Today`, `This Week`, `This Month`, `All Time`) for fast filtering.
  * **Live Search Filter**: Search attendance records by student name or PIN code.
  * **Interactive Column Sorting**: Click any report header (Log ID, User Name, Role, Check-In, Check-Out, Duration, Status) to sort.
  * **KPI Analytics Cards**: Total Students, Total Tutors, Currently Checked-In Count, Total Logged Hours.
  * **CSV Export**: Export filtered attendance logs to `.csv` spreadsheet (compatible with Excel & LibreOffice with UTF-8 BOM).
* **System Settings & Mode Parity**:
  * **Kiosk Gallery Name Sorting**: Switch between "First Name (A - Z)" and "Last Name (A - Z)" on both Desktop and Web modes.
  * **Screensaver & Lockdown Configuration**: Toggle auto-launch in screensaver lock mode or trigger Fullscreen Kiosk mode.
  * **Manager Password Management**: Update administrator password with instant validation.

## 👨‍💻 Author & Developer Support

* **Author**: Jonathan Lin
* **Support / Donations**: If this system helps your learning center or school, support development via Venmo: **`@Jonathan-Lin-630`**
