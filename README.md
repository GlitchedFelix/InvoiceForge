# InvoiceForge

**Logistics data, cleaned and grouped — automatically.**

InvoiceForge is a browser-based tool that takes raw delivery manifest data and transforms it into clean, grouped, invoice-ready Excel outputs. No server. No uploads. No manual sorting.

Built for operations and logistics teams who are tired of spending hours reconciling spreadsheets by hand.

---

## What It Does

Logistics manifests are messy. Duplicate entries, inconsistent customer names, addresses that almost-match-but-not-quite, and deliveries that need to be grouped before you can invoice. InvoiceForge handles all of that automatically.

Upload your manifest → InvoiceForge cleans, deduplicates, fuzzy-matches, and groups your data → Download a structured Excel file, ready for invoicing.

**Two modules, one tool:**

- **Store Deliveries** — Processes store-to-store and branch delivery data. Groups by customer, location, and date.
- **Partner Payouts** — Handles third-party carrier and partner delivery data. Separates output by delivery company for easy reconciliation.

---

## Key Features

- Drag-and-drop Excel upload (`.xlsx`)
- Automatic date normalisation and data cleaning
- Duplicate removal using smart reference matching
- Fuzzy grouping by customer name and delivery address
- Grouped confidence scores so you can review edge cases
- Separate output sheets per delivery company
- Downloadable Excel output — ready to send
- 100% browser-based — your data never leaves your machine

---

## How To Use It

### 1. Download the Template
Click **"Download Template"** to get a correctly formatted `.xlsx` file. Fill in your delivery data using the provided column headers.

### 2. Upload Your Manifest
Drag and drop your filled `.xlsx` file onto the upload area, or click to browse. The log panel will confirm when your file is loaded.

### 3. Generate Output
Click **"Generate Processed File"**. InvoiceForge will:
- Clean and normalise your data
- Remove duplicates
- Fuzzy-match and group similar deliveries
- Split output into separate sheets by delivery company

### 4. Download and Use
Your processed file downloads automatically as `InvoiceForge_Output.xlsx`. Open it in Excel — it's ready to use.

---

## Template Columns

| Column | Description |
|---|---|
| `Date` | Delivery or booking date |
| `Reference` | Unique shipment reference number |
| `Order_ID` | Internal order identifier |
| `Customer` | Customer or recipient name |
| `Destination` | Delivery address or location |
| `Distance_km` | Delivery distance in kilometres |
| `Weight_kg` | Shipment weight in kilograms |
| `Origin` | Sending location or warehouse |
| `Receiving_Point` | Receiving store or depot |
| `Driver_Zone` | Driver or delivery zone identifier |

---

## Privacy & Security

All processing runs entirely in your browser using client-side JavaScript. No data is uploaded to any server. InvoiceForge never sees your data.

---

## Tech Stack

- HTML5 / CSS3 / JavaScript (ES6)
- Bootstrap 5
- SheetJS (xlsx) — Excel file reading
- ExcelJS — Multi-sheet Excel output generation
- Bigram string similarity — Fuzzy matching engine

---

## About

InvoiceForge was built to solve a real problem in logistics operations — the hours lost every week manually cleaning and reconciling delivery data before it can be invoiced. It's fast, private, and requires no software installation.

Built by [Jean-Luke Pieterse](https://glitchedfelix.github.io/Personal-Portfolio-Website/) — Automation & Workflow Consultant.

---

*© 2026 InvoiceForge. MIT License.*
