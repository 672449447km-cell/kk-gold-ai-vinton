KK GOLD AI VINTON V7 — FREE AI BRAIN STARTER

WHAT THIS PACKAGE DOES
- Keeps the V6 premium gold-themed trading workspace and free XAUS XAU/USD reference quote.
- Adds a real AI-backend connection point in the AI Chat screen.
- Uses OpenRouter's free model router by default (MODEL=openrouter/free).
- Adds owner passphrase sign-in and short-lived signed sessions.
- Keeps the provider API key on the backend, not inside the phone app.
- Sends recent on-screen conversation context to the model. This starter does not provide durable personal memory across app restarts.
- The app remains gold-only for its trading features, but the AI can also answer general questions.
- The default trading risk remains 0.5%.

IMPORTANT LIMITATIONS
- This is a starter kit, NOT a deployed/connected live AI service.
- You must create your own free OpenRouter account and API key, and deploy the included Worker.
- Free model access is limited and can be slow, unavailable, changed or rate-limited.
- OpenRouter's current free model variants have a 50 requests/day limit and 20 requests/minute.
- Free models are not guaranteed to be as capable as ChatGPT.
- Image/chart understanding is not yet connected in this starter; the chart picker is only a preview.
- Browser speech input/output depends on Android Chrome support and microphone permissions.
- No AI-generated trade signal should be treated as verified without real market data and testing.
- No broker connection, trading execution, or profit guarantee.

FREE SETUP (NO PAID PLAN REQUIRED)
1. Create a free OpenRouter account: https://openrouter.ai/
2. Create an API key: https://openrouter.ai/keys
3. Create a free Cloudflare account: https://dash.cloudflare.com/
4. Create a Worker in Cloudflare and paste the contents of worker.js into its editor.
5. In Worker Settings > Variables and Secrets, add these secrets:
   OPENROUTER_API_KEY = your OpenRouter key
   OWNER_PASSPHRASE = a long, unique private passphrase
6. Optional plain-text variable:
   MODEL = openrouter/free
7. Optional security variable:
   ALLOWED_ORIGIN = the exact HTTPS origin where you host this app.
   For first tests, "*" allows any origin; change it to your app's exact origin before public use.
8. Deploy the Worker and copy its https://...workers.dev URL.
9. Host the app files (index.html, icons, manifest.webmanifest, sw.js) on HTTPS.
10. Open the app > AI Chat > Connect free AI brain. Enter the Worker URL and owner passphrase.
11. Do not share the Worker URL/passphrase with anyone. Never paste the provider API key into the app.

OWNER AND PRIVACY
- Owner recognition is by a passphrase you create, not biometric identity recognition.
- The owner session token is kept in sessionStorage and expires after 12 hours.
- Conversation history used for prompts is read from the current chat screen; no conversation database is stored by this Worker.
- The app may retain its local journal/watchlist/chat UI in browser storage depending on existing features.
- Requests are sent to OpenRouter and the selected model/provider; review provider data policies before sharing sensitive information.
- Do not send passwords, bank details, broker logins or account identifiers.
- Use a unique owner passphrase. Do not reuse your email or banking password.

FREE SERVICE LIMITS
- OpenRouter free model variants currently allow 50 requests/day and 20 requests/minute. Limits and model availability may change.
- Cloudflare Workers Free currently allows 100,000 Worker requests/day, subject to its CPU and other platform limits.
- Free does not mean unlimited, guaranteed uptime, or permanent availability.

INSTALLATION
- This remains a PWA/static web app. It must be hosted on HTTPS (or localhost) for service worker/PWA installation.
- On Android Chrome, open the hosted URL > menu > Install app / Add to Home screen.

DATA / TRADING SAFETY
- XAUS price is an indicative reference quote, not an executable broker quote.
- AI may make mistakes. Verify all market facts against reliable data.
- The 0.5% risk cap is a planning setting, not a guarantee against losses.
- This app is educational and analytical, not a licensed financial adviser.
