# DigiStano Website

Official DigiStano website for partial discharge testing, electrical diagnostics, engineering services, equipment rental, training, repair and calibration across the GCC.

## Stack

- Next.js 16 and React 19
- TypeScript
- Tailwind CSS 4
- PostgreSQL / Neon
- Resend transactional email
- Google reCAPTCHA
- Vercel hosting

## Local Development

Install dependencies:

    npm install

Start the development server:

    npm run dev

The local website will be available at http://localhost:3000.

Validate the production build before deployment:

    npm run build

## Environment Variables

Configure these variables in .env.local and in the Vercel project settings:

- DATABASE_URL
- RESEND_API_KEY
- NEXT_PUBLIC_RECAPTCHA_SITE_KEY
- RECAPTCHA_SECRET_KEY
- APPOINTMENT_TO_EMAIL
- APPOINTMENT_FROM_EMAIL
- RENTAL_TO_EMAIL

Never commit .env.local, database credentials, API keys or secret values.

## Deployment

- Repository: digistano/digistano-website
- Production branch: main
- Hosting: Vercel
- Production URL: https://www.digistano.com

The GitHub main branch is the production source of truth. Approved changes must be committed and pushed to the company repository. Vercel automatically deploys changes pushed to main.
