# BarBurrito Payroll

A clean, minimal payroll tool for BarBurrito locations. Upload Excel schedules, process hours, generate PDF reports, and split payslip PDFs - all in your browser with no server needed.

## Features

- **Multi-location** - Toggle between Brampton and Milton with separate employee lists and settings
- **Employee management** - Add, edit, delete employees with SIN hour limits and company assignments
- **Excel processing** - Upload .xlsx schedule files, auto-detect pay period
- **PDF reports** - Summary table with totals and employee breakdown
- **PDF Splitter** - Upload multi-page payroll PDFs, auto-detect employees per page, edit names, download individual payslips
- **Email drafts** - Auto-generated email with SIN hours per employee, grouped by company
- **CSV import/export** - Bulk manage employees via CSV
- **Data backup** - Export all settings and employee data as JSON
- **localStorage** - All data saved locally in your browser, no server needed

## How to Use

1. Open `index.html` in any browser
2. Select your location (Brampton or Milton) using the toggle in the top right
3. Go to **Employees** tab to set up your team (SIN hour limits and company assignments)
4. Go to **Payroll** tab, upload your Excel schedule, and hit **Process**
5. Review the preview, then generate a **PDF** or copy the **Email**
6. Go to **PDF Splitter** tab to split multi-page payroll PDFs into individual employee payslips

## Pay Rates

| Location | SIN Rate |
|----------|----------|
| Brampton | $17.55/hr |
| Milton   | $17.60/hr |

Rates can be changed in the Settings tab.

## Tech Stack

- Single HTML file, no build step
- Tailwind CSS (CDN)
- SheetJS for Excel parsing
- jsPDF + AutoTable for PDF generation
- PDF.js + PDF-lib for client-side PDF splitting
- localStorage for persistence

## Hosting on GitHub Pages

1. Push this repo to GitHub
2. Go to Settings > Pages
3. Set source to "main" branch
4. Your payroll app is live at `https://yourusername.github.io/BarBurrito-Payroll/`

## License

MIT
