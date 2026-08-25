# Lawn Blvd — Vercel + Acuity

This branch contains the Vercel-ready Lawn Blvd booking page.

- Vercel hosts the branded public website.
- Acuity Scheduling handles appointment availability, customer booking, payments, confirmations, and reminders.
- The scheduler uses owner ID 40226247.

## Deploy on Vercel

1. In Vercel, import `bossybanks/lawn-blvd-booking`.
2. Select the `vercel-acuity` branch.
3. Vercel reads `vercel.json` and publishes the static site.
4. Connect a custom domain after the first successful deployment.

Production deployment is configured for the `vercel-acuity` branch.

No Stripe keys belong in this repository. Connect Stripe inside Acuity.
