# Cat-Health-Tracker (MiauChart)

A simple, offline-first tracker for your cat's health, daily routines, and care events. It works completely offline in your browser and can be installed directly onto your Android, iOS, or desktop home screen as a Progressive Web App (PWA).

---

## Core Functions & What You Can Do

### 🐾 Multi-Pet Profiles & Pet Passport
* **Multiple Cats:** Add and switch between multiple cat profiles from the slide-out menu, each with its own independent logs, charts, and profile photo.
* **Pet ID & Emergency Details:** Expand the collapsible profile card to store your cat's date of birth (with automatic live age calculation), breed, color/markings, spay/neuter status, insurance policy, council license, vet clinic info with one-tap calling, and a **one-tap copy** button for their microchip number.
* **Local Device Photos:** Tap your cat's circular avatar to upload a photo. Photos are compressed and stored locally on your device (`localStorage`) so they never bloat your exported JSON backups.

### 📋 Comprehensive Health & Daily Care Tracking
Log entries quickly via the main **+ Log Entry** button or the **`+` shortcut** on each dashboard card:
* **⚖️ Weight Tracking:** Record weight in `kg` or `lbs` with automatic delta comparison against the previous weigh-in.
* **🥣 Daily Food Intake & Bowl Calculator:** Enter **Bowl Before (g)** and **Bowl After (g)** to automatically calculate net grams eaten, along with food type (wet, dry, raw, treats) and brand/flavor.
* **🤢 Puke Tracker:** Log episodes categorized by **Hairball**, **Food**, or **Other**, and filter counts **Per Week (7d)**, **Per Month (30d)**, or **Since a Specific Date**.
* **🧹 Litter Box Logs:** Track normal scoops and **Deep Cleans** (including cleaner presets or custom cleaner names) plus stool/urinary health tags.
* **💧 Water & Fountain Care:** Monitor bowl/fountain water levels and log refills, pump/bowl cleanings, and filter replacements.
* **💉 Vaccines & Preventatives:** Record vaccinations and flea/worming treatments with **Next Due Date** reminders and automatic overdue/upcoming alert banners.
* **🛍️ Food Purchases & 🩺 Vet Visits:** Keep track of food bags/cans purchased and general veterinary visits or grooming events.

### 📊 Interactive Trends & Searchable History
* **Health & Care Charts:** Visualize **Weight** progression, **Daily Food Intake**, and **Weekly Puke Events** with interactive charts.
* **Activity Feed:** Search by keyword or filter by category, and easily edit or delete any past entry.

### 🎨 Soft Pastel Themes & Dark Mode
* Customize the interface from the right-hand menu with a **Dark Mode** toggle and four gender-neutral soft pastel themes: **Soft Mint**, **Pastel Sky**, **Soft Lavender**, and **Airy Peach**.

---

## Run It

It is a static site with no build step: host these files from the repository root (for example, with **GitHub Pages**) and open `index.html`.

1. Place `index.html` and your round app icon named `logo.png` (recommended `120x120px` or larger square PNG) in the root of your repository.
2. Enable **GitHub Pages** in your repository settings (`Settings → Pages → Deploy from branch`).
3. Open your GitHub Pages URL on your phone and tap **Install MiauChart App** in the menu (or **Add to Home Screen** in Safari/Chrome) for full-screen offline access.

---

## Privacy, Backups & Partner Smart Merge

* **100% Local Storage:** All pet profiles and logs are saved locally in the browser on the device you use—no accounts, cloud servers, or subscriptions required.
* **Partner Smart Merge:** If you and your partner both track your cats on separate phones, export a lightweight `.json` file or copy the compact JSON text from the **Data & Partner Sync** menu. When importing on the other device, **Partner Smart Merge** compares entries per pet, detects duplicates, and consolidates new logs into one unified dataset.