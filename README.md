# How to Use the Legal Schema Generator + GEO Tool

A quick guide for using this internal tool with client sites.

## 1. Open the file

Double-click `generador-schema-legal.html` to open it in any browser. No install, no login — it runs entirely on your machine.

## 2. Fill in the client's details

The **Schema Generator** tab has six sections:

1. **Firm Details** — name, site URL, phone, address. Used for the `LegalService` schema.
2. **Lead Attorney** — name, bar credentials, law school. Same person's info applies to both languages; only specialty and practice areas have separate EN/ES fields.
3. **Reputation** *(optional)* — leave blank to skip; it won't appear in the output.
4. **Specific Page** — the URL and page name for each language version (EN and ES have separate fields, since they usually live at different URLs).
5. **Frequently Asked Questions** — use the **English / Español** toggle to switch which set you're editing. Write real, natural questions for each language — don't just translate word-for-word. Each answer should include a concrete fact or statute, since that's what AI engines end up quoting.
6. **Schema Types to Include** — uncheck any schema type you don't want in the output (Attorney, FAQPage, BreadcrumbList).

## 3. Generate

Click **Stamp document**. This builds both the English and Spanish versions at once — no need to regenerate per language.

## 4. Grab the output

In the black panel on the right:

- **JSON-LD / llms.txt** tabs switch the format.
- **EN / ES** toggle switches the language.
- **Copy code** copies whatever's currently showing.

## 5. Paste into WordPress

- **JSON-LD:** paste the whole block (including the `<script>` tags) into a header/code plugin like WPCode or Insert Headers and Footers — either sitewide or on the specific page.
- **llms.txt:** save as a plain text file named `llms.txt` and upload it to the root of that language's site (e.g. `en.clientsite.com/llms.txt` and `es.clientsite.com/llms.txt` separately, since each language version needs its own).

Repeat steps 2–5 for each new client or each new page you're optimizing.

## 6. GEO Checklist tab

Switch to **GEO Checklist** for a running list of the 5 GEO pillars (content structure, authority signals, technical setup, external consistency, multi-engine monitoring). Check items off as you complete them per client — it's a tracker, not something that feeds into the generated schema.

---

**Note:** nothing you enter is saved between sessions — closing the tab clears the form. Keep a copy of each client's generated code somewhere safe once you've pasted it into WordPress.
