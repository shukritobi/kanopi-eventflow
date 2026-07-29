# Proposal: Kanopi EventFlow

Prepared as a working concept for Kanopi Karya's event operations.

## The problem

Event organizers often manage vendor applications, participant details, payments, floor plans, documents and event-day attendance across separate Google Forms, spreadsheets and WhatsApp chats. This makes follow-up slow and creates duplicated or missing information.

## Proposed solution

Kanopi EventFlow is one event operations workspace with two connected experiences:

1. **Organizer workspace** for the Kanopi Karya team.
2. **Public registration portal** for vendors and participants.

The prototype uses Kanopi Karya Brick World as the sample event.

## Core modules

### 1. Event dashboard

- Registration, payment and task overview
- Upcoming deadlines and alerts
- Vendor application pipeline
- Daily activity and event readiness

### 2. Vendor management

- Online vendor application
- Category and booth-package selection
- Document and product-list upload
- Review, approval, rejection and waitlist workflow
- Payment-link generation and receipt status
- Booth assignment and briefing information

### 3. Participant registration

- Competition category selection
- Parent or guardian details where required
- Consent and waiver tracking
- Registration payment
- Digital ticket and QR code
- Event-day check-in

### 4. Team task management

- Event checklists
- Assignees, due dates and priorities
- Kanban workflow
- Overdue-task alerts

### 5. Floor-plan and booth allocation

- Visual booth map
- Available, reserved, pending and paid states
- Vendor placement by category and requirements
- Booth allocation export for the event team

### 6. Finance

- Vendor booth fees
- Participant entry fees
- Outstanding payments
- Refund and manual-payment records
- Payment-gateway reconciliation
- Downloadable event statement

### 7. Messaging

- Vendor approval and rejection messages
- Payment reminders
- Briefing reminders
- Participant confirmation and event-day information
- Audience filters for WhatsApp and email broadcasts

### 8. Reports

- Registration conversion
- Vendor fill rate
- Revenue and collection rate
- Registration sources
- Category mix
- Attendance and event performance

## Recommended production architecture

- **Frontend:** Next.js with TypeScript
- **Backend:** Supabase and PostgreSQL
- **Authentication:** Organizer, staff, vendor and participant roles
- **Payments:** A Malaysian FPX and DuitNow-supported gateway such as ToyyibPay, Billplz or SenangPay
- **Messaging:** WhatsApp Cloud API and transactional email
- **File storage:** Vendor documents, payment receipts, event assets and floor plans
- **QR tickets:** Signed ticket identifiers with mobile check-in validation
- **Hosting:** Vercel or Cloudflare Pages with managed database hosting

## Suggested delivery phases

### Phase 1: MVP

- Organizer login
- Event setup
- Vendor and participant forms
- Approval workflows
- Payment integration
- QR tickets and check-in
- Basic dashboard and export

### Phase 2: Operations

- Floor-plan assignment
- Team tasks
- Automated WhatsApp and email templates
- Document management
- Finance reconciliation

### Phase 3: Multi-event platform

- Reusable event templates
- Vendor accounts and application history
- Sponsor management
- Advanced reports
- Multiple organizer workspaces

## Prototype status

The repository contains a working interactive front-end preview with sample data. It demonstrates the proposed user experience and workflows. A production release would still require a secured database, authentication, live payment gateway, file storage and WhatsApp API credentials.

## Suggested outreach message

Hi Anathasha, I saw your post about developing an event-management app, so I prepared an interactive concept specifically for Kanopi Karya, using Brick World as the sample event.

The system brings vendor applications, participant registration, payments, booth allocation, team tasks, QR check-in, announcements and reports into one platform. Vendors and participants would also get a proper registration portal instead of everything being managed separately through forms, spreadsheets and WhatsApp chats.

You can explore the working preview here:

https://shukritobi.github.io/kanopi-eventflow/

This is currently an interactive prototype using sample data. The final system can be customized around your actual workflow and connected to secure login, a database, FPX or DuitNow payments and WhatsApp notifications.

Would you be available for a quick 10-minute call so I can understand how you currently manage your events and discuss how the system can be developed for Kanopi Karya?