# Asmita Jewels — deployable Next.js starter

A responsive luxury storefront with sample catalogue, category/search filters, saved shortlist, custom-design/consultation/B2B forms, server-side validation and Supabase enquiry persistence.

## Important scope boundary
This is a working website starter, not a complete jewellery ERP. Sample products, prices and imagery must be replaced/approved. Customer accounts, designer workspace, payment collection, true 3D CAD configurator, CMS integration and manufacturing/job-card system are not implemented in this release. Forms only work after Supabase is configured. Email notifications require a transactional email provider.

## Run locally
Requirements: Node.js 20+ and npm.
1. Extract ZIP and open terminal in this directory.
2. Run `npm install`.
3. Create a Supabase project.
4. In Supabase SQL Editor, run `supabase/schema.sql`.
5. Copy `.env.example` to `.env.local` and enter your Supabase URL and anon key. Set WhatsApp number using digits with country code, contact email and site URL.
6. Run `npm run dev` and open `http://localhost:3000`.
7. Submit all three forms and confirm records appear in Supabase.

## Deploy to Vercel
1. Push project to a private GitHub repository.
2. Import repository into Vercel.
3. Add the environment variables from `.env.example` in Vercel project settings.
4. Deploy and test forms on the live URL.
5. Connect your domain and set `NEXT_PUBLIC_SITE_URL` to that domain.

## Production checklist
- Add CAPTCHA/rate limiting to public enquiry endpoint.
- Configure email alerts and test delivery.
- Replace all sample images and illustrative prices with authorised assets and verified quotes.
- Publish reviewed privacy, custom-order, cancellation, shipping and returns policies.
- Configure monitoring, backups and restore tests.
- Never commit `.env.local`, service-role keys or payment secrets. Do not collect card details in these forms.
