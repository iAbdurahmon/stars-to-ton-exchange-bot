# Screenshots

Files currently used by the README:

| File | What it shows |
|---|---|
| `01-main-menu.png` | Main menu after `/start`, with the live exchange rate |
| `02-top-up.png` | Top-up flow: amount prompt, confirmation, Telegram Stars invoice |
| `03-profile.png` | Profile: language, held balance, balance available to withdraw |
| `04-withdraw.png` | Withdrawal: amount, wallet entry, memo question, confirmation |
| `05-confirmation-ru.png` | Exchange confirmation screen in the Russian interface |

Masked in the committed versions: TON wallet addresses (`04`, `05`) and the Telegram user ID (`03`).

## Still worth adding

- The successful-payout message (`✅ Payment has been successful`) following a Stars invoice
- The waitlist view, showing request date, withdrawable date and days remaining
- The admin statistics output (total users, exchanges, Stars received, TON sent)

## Before committing a new screenshot

Redact with a solid filled rectangle rather than blur — blur and pixelation can be partially
reversed. Cover:

- wallet addresses and transaction hashes
- Telegram IDs, usernames and real names other than your own
- bot token fragments, API keys, and any URL containing a key
- server IPs and hostnames
- private log/exchange channel names, if you would rather not publish them

Git keeps every committed file forever, so redact before the commit — removing an image in a
later commit does not remove it from history.

Keep images as PNG and under about 500 KB:

```bash
sips -Z 1000 new-screenshot.png
```
