# Eureka Booking

Configurable booking-request core and sales demo for Eureka Websites Tech.

Public demo after GitHub Pages is enabled: https://eurekawebsites.github.io/eureka-booking/

Mexico offer: https://eurekawebsites.github.io/eureka-booking/rescate-48h.html

US offer: https://eurekawebsites.github.io/eureka-booking/booking-rescue.html

## V1 supports
- Multiple demo business configurations from one shared core
- Services, durations and price labels
- Multiple locations and provider filtering
- Business hours, blocked dates, lead time and booking window
- Appointment-request slots
- Customer name/phone/email/notes
- Explicit request vs. confirmed-appointment distinction
- Confirmation folio
- Optional click-to-WhatsApp handoff
- Browser-local admin demo
- Mobile-first responsive UI

Proof configurations: `clinica-demo-roma`, `dental-demo`, and `spa-demo`. They are fictional and do not imply a prospect is already a customer.

## Cost guardrails
The public demo uses `localStorage` only. It sends no SMS, email, WhatsApp API message, payment or server request.

For a paying client, keep the UI and replace storage with a client-owned backend. Client pays any later metered WhatsApp API, SMS, email, payment, calendar or other provider costs.

**Automated WhatsApp/SMS is not included in the base one-time price.** Click-to-WhatsApp remains the V1 fallback.

## Before first production client
1. Production storage adapter.
2. Authenticated admin access.
3. Server-side slot collision protection.
4. Cancellation/reschedule tokens.
5. Business-specific privacy/consent copy.
6. Admin audit logging.
7. Notification adapters disabled by default.
8. Timezone/DST testing.

This is a booking-request core, not an enterprise scheduling platform. Payments, complex recurring schedules, insurance, medical records, automated WhatsApp/SMS, two-way calendar sync and marketplace behavior are separate modules.
