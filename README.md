# XYZ Fulfillment Hub

A single-page, sample-data fulfillment workflow for an e-commerce warehouse. The demo prioritizes visibility, priority deadlines, variant verification, problem tracking, and courier handoff. It does not connect to a real marketplace, inventory system, label service, or courier.

## Run locally

Open `index.html` in a modern browser. No installation or account is needed. Changes to the sample orders are saved in that browser's local storage; use **Reset demo** to restore the starting scenario. Each browser has its own independent copy.

## Demo flow

1. Choose **XYZ-1048**, start picking, and check each product, variant and quantity. **Confirm packed** unlocks after all item checks.
2. Stage the packed box, then confirm courier pickup to mark it shipped.
3. Open **XYZ-1049** to see a stock discrepancy. Resolve it to return to picking, or update its problem note.
4. Filter **Needs attention** to see priority and blocked work; search by order, customer or SKU.

## Scope and rationale

The queue makes priority work and blockers visible. Item confirmation reduces wrong-variant shipments. Explicit staging and pickup states distinguish a packed box from a handed-over shipment. Problem notes survive a page refresh on the same device. A small warehouse team can use these actions without a complex setup.

This is a demonstration, not a production order system. It has no shared multi-user state, role permissions, stock reservation, actual label generation, deadline clock, audit trail, or integrations. Real deployment would require a shared database, identity, inventory transactions, scanning, and courier APIs.
