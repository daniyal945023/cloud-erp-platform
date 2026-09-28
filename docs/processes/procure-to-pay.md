# Procure-to-Pay Process

## Process ID

P2P

## Business Objective

Enable Apex Distribution & Logistics to purchase inventory from suppliers,
receive the inventory, record supplier invoices, and settle supplier
liabilities.

## Business Scenario

Apex purchases 100 units of Product A from Supplier X at $10 per unit.

Total purchase value:

100 × $10 = $1,000

## Process Flow

1. Identify inventory requirement
2. Create purchase request
3. Create purchase order
4. Receive inventory
5. Record supplier invoice
6. Record supplier payment

## Master Data

### Supplier
Supplier X

### Item
Product A

### Warehouse
Main Warehouse

### Company
Apex Distribution & Logistics

## Transactional Documents

- Purchase Request
- Purchase Order
- Goods Receipt
- Supplier Invoice
- Payment

## Financial Flow

Goods Receipt:

Inventory increases and a receipt/clearing liability is recognized
according to the ERP configuration.

Supplier Invoice:

The supplier liability is recognized in Accounts Payable.

Payment:

The Accounts Payable liability is reduced and cash/bank is reduced.

## Acceptance Criteria

- P2P-001: Supplier can be created.
- P2P-002: Stock item can be created.
- P2P-003: Warehouse can be created.
- P2P-004: Purchase Order can be created.
- P2P-005: Inventory can be received.
- P2P-006: Supplier Invoice can be recorded.
- P2P-007: Supplier payable can be identified.
- P2P-008: Supplier payment can be recorded.
- P2P-009: Accounting impact can be identified.
- P2P-010: Inventory and financial values can be reconciled.

## SAP S/4HANA Mapping

| Business Activity | ERPNext | SAP S/4HANA |
|---|---|---|
| Supplier master | Supplier | Business Partner |
| Purchase request | Material Request | Purchase Requisition |
| Purchase order | Purchase Order | Purchase Order |
| Goods receipt | Purchase Receipt | Goods Receipt |
| Supplier invoice | Purchase Invoice | Supplier Invoice |
| Supplier liability | Accounts Payable | FI-AP |
| Payment | Payment Entry | Outgoing Payment |

ERPNext and SAP S/4HANA have different architectures and configuration
models. The mapping above is conceptual and is used for learning.