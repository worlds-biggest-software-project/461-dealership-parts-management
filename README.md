# Dealership Parts Management

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> A cloud-native parts inventory and ordering system that gives auto, powersport, and multi-line dealerships real-time stock visibility, automated reordering, and integrated core-charge tracking without the cost and lock-in of enterprise DMS platforms.

Dealership parts departments juggle thousands of SKUs across bin locations while serving service bays, retail counter customers, and OEM warranty requirements simultaneously. Existing solutions are either expensive enterprise DMS suites designed for large franchise groups or lightweight tools that lack the depth needed for serious parts operations. This project targets the underserved middle: independent and small-group dealers who need professional-grade parts management without six-figure DMS contracts.

---

## Why Dealership Parts Management?

- **Enterprise DMS pricing shuts out smaller dealers.** CDK Global and Epicor serve large franchise groups well, but their implementation cost and complexity is prohibitive for single-point and small multi-line dealerships.
- **Legacy architectures limit flexibility.** Many incumbent parts modules predate cloud-native design. CDK has been modernising, but some modules still carry legacy constraints. DIS Quantum's UI is dated compared with modern web applications.
- **Multi-brand dealers are underserved.** Dealers carrying multiple OEM brands (e.g., Kawasaki and Yamaha alongside automotive lines) need unified inventory across brands. Most solutions are optimised for single-brand franchise operations.
- **No affordable path from spreadsheets to professional tooling.** Independent multi-brand dealers who outgrow spreadsheets face a gap: lightweight inventory tools lack core tracking and OEM integration, while full DMS platforms are overbuilt and overpriced.
- **Core charge revenue leaks are common.** Without dedicated core tracking workflows -- recording charges at sale, managing returns, reconciling vendor credits, and alerting on aging cores -- dealerships lose money on unreturned cores.

---

## Key Features

### Parts Catalog and Lookup

- OEM part-number search with supersession chain resolution
- Interchange cross-referencing across OEM and aftermarket suppliers
- Fitment data integration for accurate parts identification
- Multi-line catalog support for dealers carrying multiple OEM brands

### Inventory and Bin Management

- Bin-location tracking with real-time stock levels
- Automatic stock deduction when repair orders close or counter sales complete
- Multi-site stock visibility across dealership locations
- Cycle count support and bin label printing
- Inter-site stock transfer with approval workflow and in-transit visibility

### Automated Reordering

- Reorder-point (ROP) and economic-order-quantity (EOQ) calculations
- Configurable minimum/maximum stock levels per part
- Purchase order generation for OEM and aftermarket vendors
- Vendor-specific ordering rules and scheduled price file import
- Special-order management with customer arrival notification

### Core Charge Tracking

- Core charge recording at point of sale
- Core return workflow with vendor credit reconciliation
- Aging-core alerts to prevent revenue leakage
- Core liability accounting separated from regular inventory valuation

### Pricing, Sales, and Accounting

- Pricing matrix with cost-plus, list-minus, and customer-class rules
- Counter POS with barcode scanning for high-velocity parts sales
- Accounting GL posting for parts purchases and sales without manual re-entry
- Warranty parts quarantine and return-to-vendor tracking for OEM claim compliance

### Reporting and Analytics

- Parts fill-rate and turn-rate analysis
- Obsolescence reports and stock aging dashboards
- Gross profit by part class
- Daily parts received reconciliation against purchase orders

---

## AI-Native Advantage

AI capabilities can address several pain points that incumbents handle poorly or not at all. Demand forecasting based on seasonal trends and service history can optimise reorder quantities beyond static ROP/EOQ formulas. Obsolescence prediction can identify parts at risk of becoming dead stock before carrying costs accumulate, triggering automated return or liquidation recommendations. AI-assisted supersession chain resolution can detect when an OEM part-number change should cascade across open purchase orders and repair orders, preventing orders for obsolete numbers. Counter sales assistance can suggest complementary parts or upsell items based on the primary part being purchased.

---

## Tech Stack & Deployment

The system should support cloud-hosted deployment with offline-capable counter operations that sync on reconnect -- a firm expectation in dealership environments where network outages cannot halt parts sales. OEM data integration requires EDI or API connectors specific to each manufacturer (GM Parts, Ford Parts, Mopar, ARI Parts Pro, BRP, Kawasaki, Yamaha). Barcode and QR scanning must work reliably on mobile devices in warehouse environments. A REST API is essential for third-party integrations, including CRM tools, third-party accounting systems (QuickBooks, Xero), and potential e-commerce storefronts for online parts sales. Multi-location architecture requires a shared catalog with location-specific stock levels, demanding careful database design to prevent phantom inventory.

---

## Market Context

The dealer management system and parts-specific software market is mature, with strong buyer activity across franchise auto, RV, marine, golf cart, and powersport segments (Gartner Peer Insights lists dozens of rated DMS platforms as of 2026). Enterprise platforms like CDK Global and Epicor dominate franchise dealers, while tools like DIS Quantum and BiT DMS serve niche segments. The primary barrier to entry is not software technology but OEM parts data access: accurate catalog data (part numbers, supersession chains, fitment) is sourced under commercial licence agreements with each manufacturer and must be negotiated independently.

---

## Project Status

> This project is in the **research and specification phase**.
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
