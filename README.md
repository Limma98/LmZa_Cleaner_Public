LmZa System Cleaner v1.1.0
─────────────────────────────────────────────────────
Stack     : Python (tkinter GUI) → Cloudflare Worker (JS) → Discord API
Auth      : Discord OAuth2 → guild + role check → one-time UUID token (TTL 300s)
Execution : irm {worker}/cleaner?token={uuid} | iex  [in-memory, never on disk]
Cleaning  : 32 tasks across FiveM / RedM / Windows / GPU / Discord cache
Logging   : Desktop\LmZa_Cleaner_Log.txt  +  Discord webhook on every event
Access    : guild gated
Deny log  : 
Admin     :  { secret, userId, reason } 
Versioning: GET /version  →  { version }  →  app shows update banner if mismatch

Gated with uuid checking 
