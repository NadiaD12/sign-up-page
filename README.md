# Agentix signup page

A responsive, interactive design prototype for Agentix Nexus, using the official Agentix logo, Manrope and DM Mono typography, and the navy, sapphire, and frost brand palette.

## Preview locally

Run `python3 -m http.server 8000` in this directory, then open http://localhost:8000.

## Flow

1. Enter full name, company name, company website, work email, password, and password confirmation.
2. Verify the email using preview code `123456`.
3. Choose Standard or Nexus Pro, or select **Get My Free Score** beneath the plans. Ultra is displayed as coming soon.
4. Review the simulated checkout and recurring price.
5. View the preparation transition and sample website report.

The free-score report includes a path back to plan selection.

## Prototype boundaries

This is a frontend prototype. It does not create accounts, send verification emails, process payments, or scan websites. Use sample details and passwords. Form values are held in memory only. The payment card and report findings are illustrative. Plan prices reflect the supplied design references and must be confirmed before production use.

Production integration requires authentication and email verification services, a hosted payment provider, website analysis APIs, and approved legal pages. Fonts load from Google Fonts.

## Validation

JavaScript syntax and DOM-based interaction checks passed for password mismatch, invalid verification code, account data transfer, verification, free-score navigation, Pro checkout, report rendering, and restart. Visual browser validation was unavailable in the authoring environment.

## Account entry options

The signup screen now includes **Have an account? Sign in**, **Sign in with Google**, and **Back to Agentix**. Sign-in has email/password and Google entry points. Google opens a clearly labeled demo-account dialog; selecting it during signup preserves company details and skips password/email verification for that demo identity. Back buttons return from verification, plans, checkout, and report without restarting signup.

Email and Google sign-in remain simulated. Replace `signin`, `googlePreview`, and `openDemoWorkspace` in `app.js` with the production authentication integration before launch. No Google OAuth request or password verification is implemented in this design preview.
