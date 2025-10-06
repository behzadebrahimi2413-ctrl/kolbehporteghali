Kolbeh Porteghali — Semi-real (Ready for gateway keys)
=====================================================

This package contains the same code as the mock package but includes .env.example and a payments gateway adapter stub where you can drop real credentials (Tara / Digipay / Bank).

How to run (after adding keys):
1. Copy .env.example to .env and fill the keys.
2. npm install
3. npm run dev
4. The payments/create API will attempt to build a real request (stubbed) — you'll still need to implement the provider-specific server-to-server verification and webhooks using provider docs.

Important:
- Do NOT put production keys in source control.
- For production, use a real database, HTTPS, and verify webhooks with provider signatures.
