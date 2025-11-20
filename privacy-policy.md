# Dreamer Helper's Privacy Policy

**Effective Date:** 11 November 2025  
**Last Updated:** 12 September 2025  

---

## 1. Overview
**Janvi Dreamer** (legal name *Janvi Gautam*) is the owner of Dreamer Helper, a Discord bot. The bot assigns suitable roles within the **Dreamer’s Land** Discord server after confirming whether a Discord user is a subscriber or a paid member of the **Janvi Dreamer YouTube Channel**.

This privacy statement describes in plain English what data we gather, how we use it, how we store it, and how users can remove their data at any time.

---

## 2. information
- **Owner Name:** Janvi Gautam
- **Owner Email:** janvidreamer@gmail.com, janvi@jarvibeta.xyz
- **Support Emails:** knarlix@jarvibeta.xyz, help@jarvibeta.xyz

### Official Domains
- **UI Website (Vite react):** https://dreamer.jarvibeta.xyz
- **Backend & OAuth (nodeJS):** https://srv.dreamer.jarvibeta.xyz
- **Discord auth (nextJS):** https://auth.dreamer.jarvibeta.xyz

---

## 3. Google OAuth Permissions (Scopes)
Dreamer Helper confirms YouTube membership and subscription status using *Google OAuth 2.0*.

### Scopes:
#### 1. `https://www.googleapis.com/auth/youtube.readonly`
**Purpose:**
- to ascertain if the user is a subscriber to **Janvi Dreamer's YouTube channel**.
- The channel ID, name, and URL of the profile picture are the only public channel details that are obtained.

#### 2. `https://www.googleapis.com/auth/youtube.channel-memberships.creator`
**Purpose (Completely Owner-Only):**
- This scope is only requested in cases where Janvi Gautam requests authorise herself.
- In order to assign the appropriate membership roles in Discord, it is used to view membership levels.
- Regular users are never shown or asked to use this scope. Janvi Gautam's account is the only one that uses it.

Both scopes are **read-only**. No private playlist, email address, or sensitive information is accessed.

---

## 4. Data We Collect
We only gather the bare minimum of data needed for validation.

### A. Data Stored in Our Database
- discord Id
- discord username
- youtube channel Id
- youtube channel name
- youtube channel logo (URL only)
- youtube banner image (URL only)
- **google access token** `encrypted`
- **google refresh token** `encrypted`

> Note: Before being saved, tokens are encrypted.

### B. Data Used Temporarily (Not Saved)
- User's YouTube subscription list (only to confirm subscription status)
- Owner’s channel membership members list (only to assign membership roles)

### C. When No Data Is Collected
If a user logs in **only with Discord** on the website and does **not** complete Google OAuth verification:
- No data is stored on our server.
- Only minimal Discord details are kept temporarily in the user’s browser **localStorage**.
- Once you log out or clear your browser, this temporary data is gone.

---

## 5. Purpose of Data Usage
We only use the information gathered for:
- Verifying membership and subscription on YouTube.
- Assigning or removing roles in Dreamer’s Land.
- displaying success messages for verification (along with the channel banner and DP URL).

We never share, sell, profile, or advertise using this information.

---

## 6. Data Retention & automatically deletion
Only as long as you continue to be a verified member of the server do we retain your data.

### In these situations, your data is automatically permanently erased:
- **Revocation of Google Access:**  If you remove Dreamer Helper from your Google Account permissions, your data will be erased in **24 hours**.
- **Delete Data via Discord Command:** `/verify` → press **Delete Data** → confirm → **immediate permanent deletion**.
- **Leaving Dreamer's Land Server:** Within **24 hours**, your verification data is erased.

We do not keep any logs, analytics data, or historical records.

---

## 7. User Control: How to delete Your data
You are in complete control. You can delete your data at any time.

### 1. Revoke Access (Google Recommended)
Visit: [https://myaccount.google.com/permissions](https://myaccount.google.com/permissions) Remove Dreamer Helper → data deleted within 24 hours.

### 2. Instant data deletion (Recommended)
Use the `/verify` command → press **DELETE DATA** → confirm. Deletion happens instantly.

### 3. Leave the Server (not recommended)
Within 24 hours of your leave from Dreamer's Land, your data is erased.

> Since we don't keep email addresses, identity verification might be needed if a user requests manual deletion via email.

---

## 8. Safety Procedures
We adhere to strict security guidelines:
- All of our domains are using **HTTPS**.
- **JWT + CSRF checks** protect the OAuth state.
- Prior to being stored in a database, Google access & refresh tokens are **encrypted using Node.js crypto**.
- MongoDB is protected with **TLS/SSL**.
- Verification tokens expire automatically after **10 minutes** (TTL system).
- No ads, trackers, or analytics from third parties.

---

## 9. Policy for Data Sharing
Your data is **never sold, shared, or rented by us**. Advertisers, outside companies, and other third parties are never given access to user information.

Frontend libraries used for animations or UI have **no access** to user data.

---

## 10. Children and Age Policy
Dreamer Helper is exclusively intended for Discord users.  Users under the age of **13 years** are prohibited by [Discord's rules](https://discord.com/terms#2).  We don't intentionally gather any information from kids younger than 13.

---

## 11. Law & Jurisdiction
- All operations are based in **India**.
- Data handling and servers adhere to India's IT Act regulations.
- Email-based manual deletion requests might need evidence of Discord account ownership.

---

## 12. Guidelines
Here are some guidelines for data deletion and verification:
- [verify via web portal](/guide?topic=web_verify)
- [verify via bot command](/guide?topic=cmd_verify)
- [Data deletion guide](/guide?topic=data_dlt)

These instructions give users a clear understanding of the procedure.

---

## 13. Modifications to This Policy
The Dreamer's Land Discord server will be used to notify users of any upcoming changes or additions to the privacy statement.

---

## 14. Short Summary
- For verification, only the bare minimum of YouTube data is read.
- Membership scope is strictly **owner-only**.
- No server data is stored until Google OAuth is completed.
- You can delete your data anytime with one click.
- No selling, sharing, or misuse of data.
- Fully secure, encrypted, and India-compliant.
