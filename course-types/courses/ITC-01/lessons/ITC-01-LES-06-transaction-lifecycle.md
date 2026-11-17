# ITC-01-LES-06 — International Trade Transaction Lifecycle

**Level:** Intermediate | **Study time:** 90–120 minutes  
**Languages:** English, Hindi and Thai

## 1. Learning outcomes
Map a transaction from inquiry to post-delivery closure, identify control gates, and maintain a traceable shipment file.

## 2. End-to-end lifecycle
1. **Market inquiry:** Buyer defines need, specification, quantity, destination and target date.
2. **Supplier qualification:** Verify legal identity, capability, references, product compliance and risk.
3. **Quotation:** Compare specification, price, currency, validity, lead time, delivery term and exclusions.
4. **Negotiation and contract:** Agree scope, quality, delivery, payment, remedies, governing law and dispute process with qualified advice where needed.
5. **Order confirmation:** Issue purchase order and obtain seller acknowledgement.
6. **Pre-shipment planning:** Confirm permits, classification research, origin evidence, packaging, route, insurance, booking and inspection.
7. **Production / procurement:** Track milestones, quality and changes.
8. **Cargo readiness:** Check quantity, marks, packing, dimensions, documents and inspection release.
9. **Export process:** Complete applicable export formalities and hand over cargo.
10. **International carriage:** Monitor departure, transshipment, arrival and exceptions.
11. **Import process:** Submit accurate entry, provide permits and pay applicable amounts under local rules.
12. **Delivery:** Verify delivery quantity, condition, proof of delivery and discrepancies.
13. **Payment and reconciliation:** Match invoice, order, receipt and agreed payment conditions.
14. **Closure and review:** Archive records, resolve claims and capture lessons learned.

**हिंदी:** व्यापार प्रक्रिया inquiry से शुरू होकर supplier check, quotation, contract, purchase order, shipment, customs clearance, delivery, payment और closure तक जाती है।  
**ไทย:** กระบวนการเริ่มจากการสอบถามราคา คัดเลือกผู้ขาย ทำสัญญา ยืนยันคำสั่งซื้อ เตรียมสินค้า ขนส่ง ผ่านพิธีการศุลกากร ส่งมอบ ชำระเงิน และปิดงาน

## 3. Stage gates
Do not move to the next stage until the required evidence is available:
- **Gate 1 — Supplier approval:** Identity and due diligence passed.
- **Gate 2 — Commercial approval:** Specification, price, currency and delivery terms approved.
- **Gate 3 — Compliance readiness:** Product restrictions, permits and customs-data owners identified.
- **Gate 4 — Cargo release:** Quantity, packaging and inspection evidence accepted.
- **Gate 5 — Shipment release:** Documents reviewed and booking confirmed.
- **Gate 6 — Delivery acceptance:** Receipt and exceptions recorded.
- **Gate 7 — Financial closure:** Payment and invoice reconciliation complete.

## 4. Shipment file structure
```text
ORDER-YYYY-0001/
  01-inquiry-and-quotation/
  02-supplier-due-diligence/
  03-contract-and-purchase-order/
  04-product-and-compliance/
  05-booking-and-transport/
  06-customs-and-origin/
  07-commercial-documents/
  08-insurance-and-inspection/
  09-delivery-and-claims/
  10-payment-and-closure/
```

Use access controls, versioning, retention rules and secure handling for personal or commercially sensitive information.

## 5. Milestone tracker fields
Order ID; buyer; seller; product; quantity; origin; ship-from; destination; delivery term/version/named place; planned cargo-ready date; booking number; mode; vessel/flight/truck reference; ETD; ETA; customs status; delivery date; exception owner; next action; evidence link; last updated timestamp.

## 6. Worked case
A Thai importer orders 200 pumps from a supplier in Korea. The coordinator records the approved model and serial/technical specification, confirms that the buyer has checked applicable Thai product requirements, obtains a confirmed order, tracks production, checks packing and documents, monitors the shipment, coordinates import clearance through the authorised broker, confirms delivery quantity and condition, and reconciles the invoice.

A discrepancy between the purchase order and invoice is placed on hold for correction before payment or declaration as appropriate. The coordinator does not silently edit either document.

## 7. Exception management
Use the format: **Issue → Impact → Immediate containment → Owner → Deadline → Evidence → Escalation → Closure**.

Example: ETA slips by four days. Notify buyer, check downstream production impact, obtain revised carrier/forwarder schedule, assess storage or demurrage exposure, agree mitigation, update tracker and preserve evidence.

## 8. Practical assignment
Create a lifecycle map for one import and one export. Include stage owner, input, output, control gate, deadline and evidence. Add three exception scenarios and escalation paths.

## 9. Knowledge check
1. When should product compliance be checked? **Before shipment commitment/release, early enough to obtain approvals.**
2. What proves delivery? **Appropriate delivery receipt/POD and receiving records; exact evidence depends on contract.**
3. Should discrepancies be silently corrected? **No; use authorised, traceable correction.**
4. Why maintain a shipment file? **Audit trail, coordination, claims, payment, compliance and continuity.**
