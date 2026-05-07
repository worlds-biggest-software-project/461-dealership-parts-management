# Standards & API Reference

> Project: Dealership Parts Management (461) · Generated: 2026-05-03

## Industry Standards & Specifications

### Automotive Aftermarket Data Standards

#### ACES (Aftermarket Catalog Exchange Standard)
- **Standard:** ACES Data Format
- **URL:** https://www.autocare.org/data-standards
- **Relevance:** Standardizes parts fitment data (year, make, model, engine compatibility) through the Vehicle Configuration Database (VCdb). Ensures parts fitment accuracy across dealers, distributors, and retailers.

#### PIES (Product Information Exchange Standard)
- **Standard:** PIES Data Format
- **URL:** https://www.autocare.org/data-standards
- **Relevance:** Standardizes product attributes (dimensions, weight, UPC codes, pricing, materials). Works with ACES to provide complete part and fitment information across supply chain.

#### Auto Care Association Standards
- **Standard:** Managed by Auto Care Association (formerly AAIA)
- **URL:** https://www.autocare.org/
- **Relevance:** Governance body for ACES, PIES, and other automotive aftermarket data standards. Maintains Vehicle Configuration Database (VCdb) and Product Classification Database (PCdb).

### Vehicle Identification & Diagnostic Standards

#### VIN (Vehicle Identification Number) Standards
- **Standard:** ISO 3779 (VIN Structure)
- **URL:** https://www.nhtsa.gov/vin-decoder
- **Relevance:** 17-character code identifying vehicles; used to determine parts compatibility and warranty. NHTSA vPIC API provides free VIN decoding.

#### NHTSA vPIC API (Vehicle Identification Lookup)
- **Standard:** NHTSA Open VIN Decoder
- **URL:** https://vpic.nhtsa.dot.gov/decoder/
- **Relevance:** Free federal API for VIN decoding and vehicle specification lookup; widely used in dealership parts systems.

#### OBD-II (On-Board Diagnostics)
- **Standard:** SAE J1962 (OBD-II Connector), ISO 15031-5 / SAE J1979 (OBD Protocol)
- **URL:** https://www.csselectronics.com/pages/obd2-explained-simple-intro
- **Relevance:** Diagnostic protocol for vehicle engine parameters and fault codes; used in diagnostic-based parts recommendations.

#### Unified Diagnostic Services (UDS)
- **Standard:** ISO 14229-1 (Unified Diagnostic Services)
- **URL:** https://www.csselectronics.com/pages/uds-protocol-tutorial-unified-diagnostic-services
- **Relevance:** Advanced diagnostic standard for modern vehicles; evolving alternative to OBD-II for newer vehicles with enhanced diagnostics.

### API & Data Exchange Standards

#### REST / JSON Standards
- **Standard:** RFC 7230-7235 (HTTP/1.1), RFC 8259 (JSON)
- **URL:** https://www.ietf.org/rfc/rfc8259.txt
- **Relevance:** Industry standard for API communication; used by all major parts management and dealer management APIs.

#### OAuth 2.0 Authorization Framework
- **Standard:** RFC 6749, RFC 6750
- **URL:** https://tools.ietf.org/html/rfc6749
- **Relevance:** Secure API authorization standard used by vehicle data APIs and dealer management system integrations.

#### HTTPS/TLS 1.2 and 1.3
- **Standard:** RFC 5246, RFC 8446
- **URL:** https://tools.ietf.org/html/rfc5246
- **Relevance:** Encryption standard for secure transmission of parts inventory, pricing, and customer data.

#### OpenAPI 3.1 Specification
- **Standard:** OpenAPI Initiative
- **URL:** https://spec.openapis.org/oas/v3.1.0
- **Relevance:** Standard for documenting REST APIs used in dealership parts software integrations.

#### XML / EDI Standards (Legacy)
- **Standard:** EDI (Electronic Data Interchange), EDIXML
- **URL:** https://www.edi.org/
- **Relevance:** Legacy standards still used for B2B inventory and parts ordering in automotive supply chain; increasingly replaced by REST/JSON APIs.

### Security & Compliance Standards

#### PCI DSS (Payment Card Industry Data Security Standard)
- **Standard:** PCI DSS v3.2.1 / v4.0
- **URL:** https://www.pcisecuritystandards.org/
- **Relevance:** Required for dealerships processing credit card payments for parts sales and service; dictates encryption, access controls, and payment data handling.

#### SOC 2 Type II
- **Standard:** System and Organization Controls
- **URL:** https://www.aicpa.org/interestareas/informationtechnology/sodframework.html
- **Relevance:** Independent audit standard for cloud-based parts management systems covering security, availability, and confidentiality.

#### GDPR (General Data Protection Regulation)
- **Standard:** EU Regulation 2016/679
- **URL:** https://gdpr-info.eu/
- **Relevance:** Data protection for customer vehicle information and service records in EU dealerships.

#### CCPA (California Consumer Privacy Act)
- **Standard:** California Civil Code § 1798.100 et seq.
- **URL:** https://oag.ca.gov/privacy/ccpa
- **Relevance:** Privacy rights for California customers; affects dealership data handling and customer notifications.

#### ISO 27001 Information Security
- **Standard:** ISO/IEC 27001:2022
- **URL:** https://www.iso.org/standard/81805.html
- **Relevance:** Information security management system standard increasingly required by enterprise dealerships.

### Inventory & Procurement Standards

#### UPC (Universal Product Code)
- **Standard:** GS1 UPC Barcode Standard
- **URL:** https://www.gs1.org/services/how-calculate-check-digit-manually
- **Relevance:** Standardized barcode system for parts inventory tracking and point-of-sale scanning.

#### SKU (Stock Keeping Unit)
- **Standard:** GS1 Global Trade Item Numbers (GTIN)
- **URL:** https://www.gs1.org/services/gtin-management
- **Relevance:** Unique identifier for inventory items; used in dealership parts catalogs and ordering systems.

## Similar Products — Developer Documentation & APIs

### CDK Global (Dealer Management System)
- **Description:** Market-leading DMS for dealerships with comprehensive API suite for parts, service, sales, and CRM integration.
- **API Documentation:** https://www.cdkglobal.com/cdk-global-api-solutions
- **SDKs/Libraries:** REST APIs, async APIs, data extract APIs
- **Developer Guide:** Fortellis platform with integrated API marketplace
- **Standards:** REST/JSON, OAuth 2.0
- **Authentication:** OAuth 2.0

### Fortellis (Automotive Commerce Exchange)
- **Description:** API marketplace and integration platform operated by CDK Global connecting dealers with vendors, manufacturers, and service providers.
- **API Documentation:** https://fortellis.io/
- **SDKs/Libraries:** Multiple vendor APIs on Fortellis Marketplace
- **Developer Guide:** Repair order APIs, parts APIs, service appointment APIs, F&I integration
- **Standards:** REST/JSON, OAuth 2.0, async APIs
- **Authentication:** OAuth 2.0

### Smartcar (Vehicle Data API)
- **Description:** Standardized API for accessing vehicle data across makes and models; used by dealerships for diagnostic-based recommendations.
- **API Documentation:** https://smartcar.com/
- **SDKs/Libraries:** Node.js, Python, JavaScript, REST API
- **Developer Guide:** Vehicles API, permission API, webhooks for scheduled data retrieval
- **Standards:** REST/JSON, OAuth 2.0, webhooks
- **Authentication:** OAuth 2.0 with user consent

### Auto Data (Vehicle Database API)
- **Description:** Comprehensive vehicle technical specifications and parts compatibility database.
- **API Documentation:** https://api.auto-data.net/
- **SDKs/Libraries:** REST API
- **Developer Guide:** Vehicle specifications, equipment, parts compatibility
- **Standards:** REST/JSON
- **Authentication:** API Key

### QuickBooks Online (Financial Integration)
- **Description:** Cloud accounting software for managing dealership finances, parts sales, and inventory valuation.
- **API Documentation:** https://developer.intuit.com/app/developer/qbo/docs/api/accounting-api
- **SDKs/Libraries:** Node.js, Python, Java, C#/.NET
- **Developer Guide:** Inventory tracking, vendor management, sales transactions
- **Standards:** REST/JSON, OpenAPI
- **Authentication:** OAuth 2.0

### NHTSA vPIC (VIN Decoder API)
- **Description:** Free, federal API for VIN decoding and vehicle specifications; essential for parts fitment verification.
- **API Documentation:** https://vpic.nhtsa.dot.gov/decoder/
- **SDKs/Libraries:** REST API (free, no key required)
- **Developer Guide:** VIN decoding, vehicle specifications, model options
- **Standards:** REST/JSON
- **Authentication:** None (public API)

### Shopify (E-Commerce Platform)
- **Description:** Used by dealerships for online parts selling and customer-facing parts catalogs.
- **API Documentation:** https://shopify.dev/
- **SDKs/Libraries:** GraphQL API, REST API, Node.js, Ruby, Python
- **Developer Guide:** Product catalog, inventory, orders, customer management
- **Standards:** REST/JSON, GraphQL
- **Authentication:** OAuth 2.0, API Key

### Stripe (Payment Processing)
- **Description:** Payment processor for parts sales transactions online and in-store POS systems.
- **API Documentation:** https://stripe.com/docs/api
- **SDKs/Libraries:** Python, Node.js, Java, Go, Ruby, PHP, .NET
- **Developer Guide:** Payments, billing, inventory integration
- **Standards:** REST/JSON, OpenAPI 3.0
- **Authentication:** API Key (live/test), OAuth 2.0

### Google Workspace APIs (Business Tools)
- **Description:** Email, calendar, and documentation for dealership staff collaboration.
- **API Documentation:** https://developers.google.com/workspace
- **SDKs/Libraries:** Python, Node.js, Java, C#/.NET, Go, Ruby
- **Developer Guide:** Gmail API, Calendar API, Drive API
- **Standards:** REST/JSON, OAuth 2.0
- **Authentication:** OAuth 2.0

### Zapier (Integration Platform)
- **Description:** No-code integration platform connecting dealership systems, accounting software, and customer communication tools.
- **API Documentation:** https://zapier.com/platform/
- **SDKs/Libraries:** JavaScript/Node.js for custom integrations
- **Developer Guide:** Zapier Platform API for custom integrations
- **Standards:** REST/JSON, webhooks
- **Authentication:** OAuth 2.0, API Key

## Notes

### Gaps and Challenges in Parts Management Standards

1. **VIN to Parts Mapping:** While VIN decoding is standardized (ISO 3779), real-time VIN-to-parts compatibility requires proprietary databases (ACES/PIES). No single API standard exists; dealerships often integrate multiple data sources.

2. **OBD-II Adoption in DMS:** OBD-II diagnostic protocols are not universally integrated into dealer management systems; most dealerships still manually reference diagnostic codes for parts recommendations.

3. **EDI Legacy Integration:** Many parts suppliers and distributors still use EDI (Electronic Data Interchange) for ordering; modern REST/JSON APIs are gradually replacing this but coexist in the industry.

4. **Real-Time Inventory Sync:** No standard protocol exists for real-time inventory synchronization between dealership parts systems and manufacturer/supplier systems; most use batch updates or custom integrations.

5. **Warranty Data Integration:** Warranty claim data and parts traceability are not standardized across manufacturers; dealerships must integrate with individual OEM systems.

6. **Pricing Variability:** Parts pricing varies by supplier, dealer tier, and volume; no standard pricing API exists across the industry.

### Regulatory & Compliance Considerations

1. **PCI DSS:** Critical for any dealership accepting credit cards for parts sales; cloud-based systems must maintain current SOC 2 compliance.

2. **CCPA/GDPR:** Growing requirement as dealerships manage customer vehicle data and service history.

3. **Vehicle Recall Information:** Some dealerships integrate NHTSA recall data to recommend parts for safety recalls; no standardized API exists.

### Technical Recommendations

1. **Implement ACES/PIES Integration:** Essential for accurate parts fitment; use established ACES/PIES data feeds or integrate via Auto Care Association-certified partners.

2. **Use REST/JSON APIs:** Modern REST APIs with OAuth 2.0 provide better interoperability than legacy EDI; prioritize APIs that support OAuth 2.0.

3. **Integrate NHTSA vPIC:** Free VIN decoding provides a foundation for parts compatibility; consider supplementing with commercial vehicle databases for enhanced fitment data.

4. **Support Multiple Payment Gateways:** Stripe, Square, and PayPal integrations provide flexibility for parts sales online and in-store POS.

5. **Plan for OBD-II/UDS Integration:** Future versions should support diagnostic-driven parts recommendations; this will become increasingly important as vehicles shift to connected architectures.

6. **Maintain SOC 2 Compliance:** Essential for cloud-based parts management systems serving multiple dealerships.

7. **Consider MCP Server Integration:** For AI-powered features like predictive parts demand, warranty optimization, and customer vehicle health recommendations.

### Emerging Trends

- **Connected Vehicle Data:** OEMs increasingly offer APIs to dealerships for real-time vehicle health monitoring, enabling proactive parts sales
- **AI-Driven Recommendations:** Integration with vehicle diagnostic APIs (like Smartcar) + ACES/PIES for AI-powered parts recommendations
- **Supply Chain Visibility:** Real-time supplier inventory and lead time data to optimize dealership parts ordering
- **Electrification:** New parts standards emerging for EV-specific components and battery diagnostics
