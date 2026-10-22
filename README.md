# RentWise

RentWise is a local-first landlord and property-management dashboard for Kenya. It tracks properties, units, tenants, rent, receipts, maintenance requests, and basic reports in Kenyan shillings.

## Run it

1. Open the `RentWise` folder in VS Code.
2. Install the **Live Server** extension if you do not have it.
3. Right-click `index.html`, then choose **Open with Live Server**.
4. Use **Load demo data** in the dashboard to explore it safely.

## Files

- `index.html` contains the landing page, dashboard shell, forms, and dialogs.
- `style.css` contains the visual design and responsive mobile layout.
- `script.js` contains the data model, calculations, form validation, safe rendering, receipts, and localStorage persistence.

## Data and safety

This is a frontend prototype. Data stays in the browser through `localStorage`; clearing browser site data also clears RentWise data. It has no M-Pesa, bank, login, cloud, or real SMS connection. User-entered text is escaped before the app renders it.

## Production upgrade path

For a real service, add a backend API and database (for example Node.js/Express + PostgreSQL), authenticated landlord and tenant accounts, role-based permissions, backups, audit logs, and HTTPS. Put payment integration exclusively on the backend using an approved M-Pesa provider; never place secrets, private keys, or payment credentials in browser JavaScript. Add SMS/WhatsApp only with consent and compliant providers.
