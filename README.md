# Student & Tutor Check-In & Check-Out Kiosk System

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
* **Visual Gallery Selection**: Students and tutors can tap/click their name card directly from a visual gallery or use the search bar/role filter (`All`, `Students`, `Tutors`).
* **Dual PIN Input (Touch Keypad & Keyboard)**: Enter PIN using either the touch on-screen numeric keypad or physical keyboard (top-row numbers, numpad, `Backspace` to edit, `Enter` to confirm, and `Escape` to cancel).
* **Instant Confirmation**: Audio/visual feedback banners confirm check-in and check-out status and calculate total session time.

### 2. Lock Screen / Kiosk Saver
* **Password-Protected Fullscreen Kiosk Mode**: Intercepts shortcut keys and locks the screen into fullscreen mode.
* **Manager Passcode Protection**: Prevents kids or unauthorized users from closing the app or navigating away without entering the Manager Password (default: `admin123`).

### 3. Manager Admin Dashboard
* **User Management (CRUD)**: Add, edit, remove, or reset PINs for students and tutors.
* **Bulk CSV Import**: Import student/tutor records from any custom `.csv` file with interactive **Field Mapping** (maps Full Name, Role, Age, and PIN Code columns, with automatic 4-digit PIN generation for missing codes).
* **Attendance & Duration Reports**:
  * Date range selector (Start Date to End Date).
  * Role filter (`All`, `Students`, `Tutors`).
  * KPI Analytics Cards: Total Students, Total Tutors, Currently Checked-In Count, Total Logged Hours.
* **CSV Export**: One-click export of attendance logs to `.csv` spreadsheet (compatible with Excel & LibreOffice).
* **Settings**: Change Manager Password and configure kiosk preferences.
