# Sewangan Admin — Full Build

This repository implements the complete 40-area ERP structure requested for Sewangan:
login/security, dashboard, organization, members, employees + joining documents + T&C, volunteers, beneficiaries, help/charity, money/goods donations, collection, donors, fundraising, programs, projects, events, campaigns, attendance, leave, accounts/transactions/cash book/bank book/ledger, payments, receipts, vouchers, expenses, inventory, purchases, vendors, assets, documents, letters/dispatch, certificates, meetings, notifications, reports, global search, settings, English/Hindi selector, responsive UI, role permissions and shared data infrastructure.

All register modules use schema-driven Add/Edit/View/Delete/Approve/Search/Filter/Print/CSV controls subject to permissions. Settings includes UPI ID + payment QR upload. Receipt numbering is six digits: SDR/2627/000001.

Deployment:
1. Import `docs/Sewangan_ERP_Full_Database.xlsx` into Google Sheets.
2. Open Extensions > Apps Script and add backend files.
3. Run `setupSewanganERP()` once.
4. Change seeded `CHANGE_ME_NOW` immediately.
5. Deploy Apps Script as Web App and paste its URL into `config.js`.
6. Publish this repository using GitHub Pages/your hosting.

Production hardening still required before real sensitive KYC/payment use: password hashing or external auth, server-side payment verification/webhooks, restricted file storage, encryption/access controls and backup policy.
