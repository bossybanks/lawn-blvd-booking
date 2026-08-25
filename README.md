# Lawn Blvd Booking Site

Railway-ready lawn-service booking, Stripe Checkout, add-on services, PostgreSQL appointment storage, and a password-protected booking dashboard.

## Railway setup

1. Deploy this GitHub repository in Railway.
2. Add a PostgreSQL service to the same Railway project.
3. Set `DATABASE_URL=${{Postgres.DATABASE_URL}}` on the app service.
4. Add secret variables: `STRIPE_SECRET_KEY`, `STRIPE_WEBHOOK_SECRET`, and `ADMIN_PASSWORD`.
5. Add `PUBLIC_URL` with the complete deployed URL, such as `https://book.lawnblvd.com`.
6. Add `book.lawnblvd.com` under the app service's **Settings → Networking → Custom Domain**.
7. In Stripe, create a webhook at `https://book.lawnblvd.com/api/stripe/webhook` for `checkout.session.completed` and `checkout.session.expired`.

The customer page is `/`. The protected booking list is `/admin.html`.

Never commit Stripe keys or passwords to the repository.
