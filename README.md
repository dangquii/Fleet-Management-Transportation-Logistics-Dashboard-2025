# Fleet Management Transportation & Logistics Dashboard 2025

An Excel-based analytics solution that turns raw freight trip records into an interactive, single-page control tower.  
It reveals cost drivers, labour mix, trip productivity and cargo utilisation—without requiring any paid BI platform.
![Interactive freight dashboard](images/dashboard.png)


---

## Problem Addressed  
Small-to-mid-sized carriers often run their fleets from spreadsheets, leaving decision-makers blind to empty-mile cost, labour overruns and seasonal expense spikes. Industry studies estimate **20–35 %** of truck kilometres are still driven empty and that fuel + labour routinely consume **65–70 %** of total operating cost. This dashboard converts everyday trip logs into actionable KPIs so managers can close those gaps.

---

## Key Metrics Visualised
| Category | KPIs |
|----------|------|
| **Trips** | Total trips, one-way vs return count, outsourced (hired) trips |
| **Distance** | Aggregate km, distance per cargo type, distance per trip class |
| **Cargo Types** | Shipment counts & km share (e.g., Woodchip vs Woodpellet) |
| **Cost** | Total expenses, salary vs wage mix, monthly spend trend |
| **Labour** | Driver & buddy wage tiles with sparklines, salary cards |
| **Productivity** | Expenses / km, trips / month, income per trip class |

---

## Features
- **Single-screen dashboard** with KPI cards, donut gauges, sparklines, bar & line charts.
- **Interactive slicers** for Driver, Month and Trip Class—no VBA, no add-ins.
- **Calculated fields** surface on-time %, hired-transport cost delta, one-way vs return efficiency.
- **One-click PDF export** for board packs; file opens read-only in any modern Excel install.
- **Clean UI theme** (rounded tiles, soft shadows) modelled on enterprise BI design.
  
---

## Requirements
| Software | Version |
|----------|---------|
| **Microsoft Excel** | 365 or 2019+ (Windows or macOS) |
| **Memory** | < 50 MB RAM while open |
| No macros or external libraries required.

---

## Quick Start  

1. **Download** or clone this repo.  
2. Open `Freight Excel Dashboard Analysis.xlsx`.  
3. If prompted, **enable editing** (read-only is fine for viewing).  
4. Use the slicers on the left panel to filter by driver, month or trip class.  
5. Export a PDF: **File → Export → Create PDF/XPS → Active Sheet**.

---

## Data Schema (`sample_freight_dataset.csv`)

| Column | Sample | Description |
|--------|--------|-------------|
| `order_id` | ORD10017 | Unique trip identifier |
| `order_date` | 2025-02-14 | Trip start date |
| `driver` | Antoni | Lead driver |
| `distance_km` | 65 | Total kilometres |
| `trip_class` | Return / One-Way / Close / Far / Regular |
| `cargo_type` | Woodchip | Commodity hauled |
| `weight_kg` | 12 000 | Payload weight |
| `driver_wage` | 600 VND | Wage per trip |
| `buddy_wage` | 100 VND | Assistant wage |
| `driver_salary` | 800 VND | Fixed salary allocation |
| `hired_transport` | Yes/No | Outsourced carrier flag |

---

## Business Value
- **5–15 % logistics-cost reduction** potential by spotlighting high-cost lanes, empty-mile exposure and overtime spikes.  
- **Faster decisions**: finance, operations and fleet planning share one live source of truth.  
- **Scalable**: same model can connect to SQL/Power BI when row counts grow.
