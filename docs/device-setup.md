# 📱 Set Up Business Email on Android, iPhone & Outlook

[← Back to Business Email Setup](../README.md)

Have these ready:

```text
Email:     you@yourbusiness.co.ke
Password:  ••••••••••
Server:    mail.yourbusiness.co.ke
IMAP:      993  (SSL/TLS)
SMTP:      465  (SSL/TLS)  — or 587 (STARTTLS)
```

---

## 🤖 Android — Gmail app

1. Open **Gmail** → profile picture → **Add another account** → **Other**.
2. Enter your full email → **Manual setup** → **Personal (IMAP)**.
3. Password → **Next**.
4. Incoming server: `mail.yourbusiness.co.ke`, port `993`, security **SSL/TLS**.
5. Outgoing server: `mail.yourbusiness.co.ke`, port `465`, security **SSL/TLS**, *Require sign-in* ✅.
6. Choose sync frequency → **Done** 🎉

## 🍏 iPhone / iPad — Mail app

1. **Settings → Apps → Mail → Mail Accounts → Add Account → Other → Add Mail Account**.
2. Name, full email, password, description → **Next**.
3. Choose **IMAP**.
4. Incoming host: `mail.yourbusiness.co.ke` · username: full email.
5. Outgoing host: `mail.yourbusiness.co.ke` · username: full email · password.
6. **Save**. If asked about the certificate, make sure the server name matches your domain.

## 🪟 Outlook (Windows / Mac — new Outlook)

1. **File / Settings → Accounts → Add account**.
2. Enter your email → **Advanced options → Let me set up my account manually** → **IMAP**.
3. Incoming: `mail.yourbusiness.co.ke`, `993`, SSL/TLS.
4. Outgoing: `mail.yourbusiness.co.ke`, `465`, SSL/TLS.
5. Enter password → **Connect**.

## 🔁 Read business mail inside your existing Gmail (desktop)

Gmail → ⚙️ **See all settings → Accounts and Import → Add a mail account** → POP3/IMAP details above. Then **Send mail as** → add your business address using SMTP `465` SSL.

---

| Symptom | Fix |
|---|---|
| 🔴 "Cannot verify server identity" | Use `mail.yourbusiness.co.ke` (or the host's server name) exactly; ensure SSL is installed on the mail hostname |
| 🔴 Sends fail on Safaricom/office Wi-Fi | Switch SMTP to port `587` + STARTTLS |
| 🔴 Duplicates / missing folders | You used POP3 — remove the account and re-add as IMAP |

> 🛟 Need help? [HostingKE Knowledge Base](https://hostingke.co.ke/knowledge-base) · [Help Center](https://hostingke.co.ke/help-center)
