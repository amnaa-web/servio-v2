# Servio Marketplace MVP — V2

An incremental upgrade of the original Servio prototype. The design system, branding and HTML/CSS/JavaScript deployment style are retained. No npm build or API credentials are required.

## Features

- **Customer:** browse and filter services and realistic fictional provider profiles; three-step booking (service → provider → schedule → confirmation); demo slot availability; booking status/history, cancellation and detail timeline.
- **Service Provider:** choose a simulated provider identity and accept, reject, or complete assigned bookings. Statuses reflect in the customer and admin workspaces.
- **Admin:** manage customers (add, enable/disable), services (add, edit, enable/disable), providers (add, edit, enable/disable), applications (approve/reject), and booking records. Search records and reset demo data.
- **UX:** responsive sidebar/mobile navigation, notifications, modal forms, filters, success/error states, empty states and simulated action delay.
- **Support:** sample support request form.

## Deployment

Upload `index.html`, `app.js` and `vercel.json` to a GitHub repository and import it into Vercel. Choose **Other** as the framework, set root to repository root, and leave build command unset. Alternatively, open `index.html` directly in your browser.

## Demo instructions

1. In **Customer**, pick a service and then a provider; choose an available date/time; submit the booking request.
2. In **Service Provider**, use the selector to switch to that provider; accept or reject the request.
3. Return to **My Bookings** to see the updated status, or open **Admin Console** for management and activity.
4. Use **Admin Console → Reset demo** to restore original sample data.

## Important limitations

Everything, including users, bookings and bookings statuses, is stored in **localStorage in this one browser**; there is no backend, database, multi-user synchronization, secure login, real provider verification, real payment processing, map tracking, notifications, actual scheduling systems, or identity assurance. The displayed ratings, customers, providers, booking metrics, prices and earning figures are fictional. Dates/availability are only demo rules. The UI includes no actual authentication or authorization. Do not use this as a real service or submit real personal information.

**Production next steps:** real customer/provider/admin auth and RBAC; shared backend and database with transactional availability locking; KYC; payment gateways and payment webhooks; notifications, maps, refunds, audit logs, and iOS/Android apps; automated and device-level testing.
