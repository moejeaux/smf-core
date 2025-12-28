# SMF SDK Test App

You are an external integrator testing the `@smf/sdk` package from `../smf-core`.

Constraints:
- Only use this README and the public `@smf/sdk` API.
- Do NOT inspect `../smf-core` source.

Tasks:
1. Create a minimal Next.js or Express app in this folder.
2. Implement a `/pay` endpoint that:
   - Uses SMF test mode.
   - Performs a test charge with a test token and amount.
3. Implement a webhook endpoint that:
   - Verifies signatures using `verifyWebhookSignature` from `@smf/sdk`.
   - Logs successful `payment.succeeded` events.
4. Provide simple instructions in this README for running:
   - The server.
   - A test charge.
   - Webhook testing with a tunnel (e.g., ngrok).
