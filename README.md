# Inland Waterway Logistics Dashboard

This repository contains the **Inland Waterway Logistics (IWL) Dashboard**, an interactive tool for modelling the economics of Freight ‑as‑  Service (FaaS) operations on urban waterways.  The dashboard is part of the Belgium Autonomous Cargo initiative and supports investors, operators and municipalities in evaluating the potential of autonomous, electric cargo vessels for last ‑mile logistics.

## Background

Urban waterways are an under ‑used transportation corridor that can help relieve road congestion and reduce greenhouse‑gas emissions.  The Belgium Autonomous Cargo project proposes to retrofit small barges with electric propulsion, autonomy kits and remote control, and to operate them as a fleet serving city construction sites, retailers and waste logistics.  Each vessel can replace multiple trucks and operate quietly at night, delivering materials and returning waste.

To attract partners and investors, the project team developed a value‑chain based business model covering:

* **Infrastructure** — quays, smart terminals, charging/battery‑swap stations, and a digital‑twin training centre.
* **Vessel layer** — retrofit of existing barges (15‑20 m) with electric propulsion, bow/stern thrusters, sensors, autonomy and 5G connectivity.
* **Control layer** — remote command centre, mobile remote‑control consoles and handheld devices, enabling autonomy levels 2‑4.
* **Data & AI** — sensors for riverbed scanning, water and air‑quality monitoring, GNSS/RTK positioning and real‑time environment data.
* **Operations** — cargo delivery (construction materials, retail goods, parcels) and back‑haul waste return.
* **Customers** — construction companies, ports, cities and water authorities.

The financial model includes revenue streams from freight (ton‑kilometre fees, fixed trip fees), subscriptions, data services and training fees, while costs include CapEx for retrofits and infrastructure, energy consumption, maintenance, remote operations, data/AI Opex and port fees.  Key metrics such as payback period, annual EBITDA, net present value (NPV) and internal rate of return (IRR) are used to assess profitability.

## About the dashboard

The interactive dashboard provided in `index.html` (originally named `uwl_faas_model.html`) allows you to:

* Adjust core assumptions (price per ton, load factor, number of trips, energy cost, crew cost, etc.).
* Model additional cost categories (infrastructure, data & AI, control & admin CapEx, data/AI Opex, docking fees) and non‑freight revenue (training, data services).
* Visualise per‑trip margins, annual EBITDA, payback period, NPV and IRR.
* See monthly cash‑flow charts, cumulative cash curves, revenue/cost mixes and sensitivity analysis.
* Export scenarios or share a link for further analysis.

The dashboard runs entirely in the browser, without any backend, and can be deployed via GitHub Pages.

## Repository layout

```
/
├── index.html       — interactive dashboard (based on the FaaS profit calculator)
├── js/              — optional JavaScript modules (if split from the main HTML)
├── data/            — optional CSV or JSON data for default cost assumptions or historical records
├── README.md        — this overview and usage guide
└── .github/workflows/ (optional) — continuous deployment via GitHub Actions
```

## Getting started

To use the dashboard locally, open `index.html` in a modern web browser.  For deployment on GitHub Pages:

1. Ensure this repository is public (or enable Pages for private repositories).
2. In repository settings, enable **GitHub Pages** from the `main` branch and select the root folder.
3. (Optional) Set your custom domain (`www.cxg111.me`) in the Pages settings and update your DNS records accordingly (use `A` records for the apex domain and a `CNAME` record for `www` as recommended by GitHub【983117945205674†L60-L87】【348268540629840†L83-L169】).
4. Commit and push changes; GitHub will automatically build and deploy your site.

Contributions are welcome via pull requests or issues.
