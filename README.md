# ⚡ Git-Nostr Bridge 

**Git collaboration, without the platform.**

This automated daemon bridges the decentralized web with GitHub. It listens for `git` patch events on Nostr and syncs them to the main [Flokicoin Repository](https://github.com/flokiorg).

## 🚀 Submit a Patch via Nostr

Use the `ngit` CLI to route patches to this bot.

**1. Install `ngit`**  
Get the CLI and documentation at [gitworkshop.dev/ngit](https://gitworkshop.dev/ngit).

**2. Broadcast your patch**  
Use `ngit` to generate and publish your patch. 

**3. Supported Relays**  
Ensure your events broadcast to our monitored relays:
* `wss://relay.ohstr.com`
* `wss://relay.damus.io`
* `wss://relay.primal.net`

## 🔐 Verification & Contact

* **Flokicoin Main Repo:** [github.com/flokiorg](https://github.com/flokiorg)
* **Bot Identity:** To grab the Nostr identity (npub/nip05) of the bot, reach us at **git@flokicoin.org**

## ⚙️ How it works

1. **Listens:** Maintains WebSocket connections to configured Nostr relays.
2. **Filters:** Monitors for NIP-34 patch events targeting the Flokicoin repository.
3. **Applies:** Pulls the raw patch and applies it locally, preserving the author's name and email.
4. **Pushes:** Pushes the commit to GitHub, appending the Nostr Event ID for cryptographic verification.

---
*Bot account. Do not send DMs or PRs here.*
