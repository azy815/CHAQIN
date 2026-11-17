# Security

Do not commit Supabase service keys, Cloudflare tokens, administrator passwords, token secrets, exported records, student information, or photos.

All production secrets must be supplied through Cloudflare Worker secrets. If a secret is exposed:

1. Rotate the Supabase key and administrator password.
2. Regenerate `TOKEN_SECRET`.
3. Redeploy the Worker and invalidate existing sessions.
4. Review database access logs and submitted records.

For security issues, contact the repository owner privately instead of opening a public issue containing exploit details.
