# Kanopi EventFlow

An interactive front-end concept for a complete event management system, tailored to Kanopi Karya's pop-up events and Brick World competition in Miri, Sarawak.

## Live preview

Open `index.html` in a browser, or use the hosted preview link provided with the repository.

## What is included

### Organizer workspace

- Multi-event dashboard
- Vendor application pipeline
- Vendor documents, approval, booth and payment status
- Participant and tournament registration
- QR-style event-day check-in simulation
- Task management and pre-event checklist
- Visual booth and floor-plan assignment
- Payment tracking and reconciliation dashboard
- WhatsApp and email message templates
- Reports and event forecasts
- Team, branding and workspace settings

### Public event page

- Event landing page
- Competition categories
- Vendor packages
- Vendor application form
- Participant registration form
- Registration-to-payment flow preview
- Event FAQ and visitor information

## Demo interactions

- Navigate between all organizer modules
- Search and filter vendors and participants
- Add vendors, participants, tasks and events
- Check in participants
- Select booths and inspect assignments
- Switch to the public event page
- Open vendor and participant forms
- Export sample CSV reports
- Preview message templates and scheduled broadcasts

## Production architecture recommendation

- Frontend: Next.js or React with TypeScript
- Backend: Supabase or PostgreSQL with row-level security
- Authentication: organizer, staff, vendor and participant roles
- Payments: ToyyibPay, Billplz, SenangPay or another Malaysian FPX/DuitNow provider
- Messaging: WhatsApp Cloud API plus transactional email
- Storage: vendor documents, receipts, floor plans and event assets
- QR: signed ticket tokens with mobile check-in validation
- Reporting: event-level finance, attendance and conversion metrics

## Important note

This repository is a working interactive prototype using sample data. It demonstrates the full user experience and system flow, but it does not yet include a production database, authentication, live payment processing or WhatsApp API credentials.
