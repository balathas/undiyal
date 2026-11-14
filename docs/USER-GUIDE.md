# Undiyal (உண்டியல்) – Family Finance & Records

An *undiyal* is the little savings box many of us had as children. Undiyal is a personal, goal-based family finance tracker that runs entirely in your web browser. It is a single file, `Undiyal.html`. There is nothing to install and no account to create, and your data never leaves your computer.

## What it does

- Tracks what you own (mutual funds, stocks, PF, PPF, deposits, savings) and which goal each holding is for.
- Shows how far along each goal is (retirement, children's education, house, emergency fund and so on), how much you need to invest each month, and whether the mix of equity and debt suits the time left.
- Keeps a history of your total savings through monthly snapshots.
- Tracks your loans (EMIs, principal still owed and interest still to pay) so net worth stays accurate.
- Stores important family details (insurance, bank accounts, deposits, ID documents) with scanned documents attached, and reminds you of upcoming premiums, maturities and expiries.
- Creates a simple, plain-language summary to share with your family, or a detailed report for an adviser with the sections you choose (**Reports ▾** at the top), as an HTML file or PDF.

## Where it works

- **Works:** computers (Windows, Mac, Linux) in Chrome, Edge, Firefox or Safari, and Android phones in Chrome.
- **Does not work on iPhone or iPad.** The Files app only previews HTML files without running them, so you see a blank page or a "can't run here" message, and no iPhone browser can open a file saved on the phone. Use a computer or an Android phone instead.

## Your data and privacy

- **Everything is kept in one JSON file on your computer or phone** (for example `undiyal-data.json`). The tracker never uploads anything.
- **Chrome and Edge on a computer, and Chrome on Android,** save every change straight to that file and remember which file you used, so you can continue with one click next time. Only a reference to the file is remembered, never its contents. Next time, click **Continue with undiyal-data.json** (or press Enter) and allow access when Chrome asks. Browsers always need this one click for a file opened from your computer or phone.
- **Firefox, Safari and older phone browsers** cannot write to files. A bar at the bottom shows "Unsaved changes" with **Save data**, which downloads `undiyal-data.json`: replace your old file with it (the browser may name a repeat download `undiyal-data (1).json`; next time, open the newest one). Until you save, your changes are kept in this browser on this device, so they survive closing the tab; next time the start screen offers to recover them. Snapshots and documents are inside that file.
- **Set a passphrase** (Settings → Your data file) if the file holds personal details or documents. The whole file is then encrypted (AES-256). If you forget the passphrase, the file cannot be opened.
- **Header buttons.** Chrome and Edge: **Save data** until you have chosen a file, then only **Back up data** (every change already saves to your file). Firefox and Safari: **Save data** and **Back up data**. On a phone they are in the ⋯ menu.
- **Back up data** downloads a dated copy, `undiyal-backup-YYYY-MM-DD.json` (year first, so backups sort in date order), and you stay on your current file. Keep it somewhere other than this computer, such as a USB drive or a cloud folder. The dashboard reminds you if you have not backed up in 30 days, and Settings → Your data file shows the date of your last backup. **Save as new file** (Chrome and Edge, in Settings) is different: it moves your work to a new file.

## Getting started

1. Open `Undiyal.html` on a computer in Chrome, Edge, Firefox or Safari, or on an Android phone in Chrome (not iPhone or iPad). Click **About** (top left) for a plain-language introduction you can show your family.
2. The start screen has a **Preferences** bar at the top: **Language** (changes the start screen and the setup wizard straight away), **Number format** and **Currency symbol** (used when you start a new file; a file you open keeps its own settings). Below it are two cards:
   - **Left:** **Continue with undiyal-data.json** (or press Enter) if you have used Undiyal before in this browser, or **Open your data file** (click the box or drop your JSON file onto it). **Open a different file** and **Forget this file** are here too.
   - **Right, Start something new:** **Start the setup wizard**, or **Try it with sample data** to look around first. Sample data is never saved unless you choose Save data.
3. The **setup wizard** first shows a short note, once per data file: Undiyal is not financial advice, the figures are estimates, and your data stays on your device. Click **OK, got it** to continue. It then takes seven steps:
   1. **Preferences:** language, number format and currency symbol (filled in from the start screen). Everything else, such as expected returns, the equity level for long-term goals, reminders, dashboard charts, theme and text size, keeps sensible defaults; change it any time in **Settings** after setup.
   1. **About you (optional):** names and ages for you and your spouse, and children's names and birth years. Ages fill in goal years and are shared with the retirement calculator (change them in either place); names show whose each holding is.
   2. **Goals:** add what you are saving for. Each row has **Cost today** and **Cost when due**: you type one, and the other is worked out (shown in a grey box). For most goals you type today's cost; for retirement you type the corpus you need at retirement, or use **Not sure? Calculate corpus**. If you are continuing a plan made in an earlier year, tick that option and enter the costs as you worked them out then; the tracker adds inflation up to today.
   3. **Holdings:** import your CAS statement for mutual funds, upload a CSV for everything else, or type holdings in.
   4. **Loans (optional):** add your loans, or click *I have no loans*.
   5. **Assign:** pick the goal each holding is for, or split it across several goals. **Suggest goal splits** can fill this in for you.
   6. **Finish:** choose where to keep your data file (Chrome and Edge), or let it download (other browsers). This opens the dashboard and saves your first snapshot. Nothing asks for a file before this step; until then your progress is kept on this device.

## Editing

Holdings, Goals and each Important section are read-only until you click **Edit**. Changes save as you type. **Done** keeps them; **Cancel** puts back everything as it was when you clicked Edit (with Undo, in case you cancel by mistake).

## Reading your dashboard

- **The header** has three numbers: **Saved so far** (with the share of what you need), **Needed by the goal dates** (with the cost in today's prices) and **Invest each month**, then a progress bar and one line on what today's savings grow to on their own. **Show the details** has the rest (what falls due within 5 years, in 5–15 years and later, the share of today's cost already saved) and *How is this worked out?*.
- **Your next steps** lists up to three things worth doing now, for example a goal that is far behind, money not yet assigned to a goal, the amount to invest each month (or as a lump sum or yearly), or goals to rebalance.
- **Each goal's label** says where it is heading: *On course*, *Almost there*, *Getting there*, *Early days*, *Not started*, or *Far behind* (a goal less than 2 years away running out of time). A goal card shows how much of the target is saved now, and a line such as "Your current investments will reach 106% of the target by Mar 2048": how far today's savings get on their own by the goal date.
- **Still to cover** is the part of your goals that today's savings won't reach on their own, even after growing.
- **Monthly needed** includes what you already put in regularly, such as mutual funds, PF and PPF.
- **Explain this page** (next to the tabs, or in the ⋯ menu on a phone) gives a short guided tour of the Dashboard, Holdings, Goals, Loans, Corpus and Important tabs, using your own numbers. With no data yet, it can show the tour with sample data without saving anything.

## Family members and joint holdings

Each holding has an **owner**: you, your spouse, a child, or **Joint**. Goals and the Dashboard always use the whole family's money together. The owner only records whose name a holding is in.

- **Importing statements for two people:** import each person's CAS one after the other. Undiyal reads the name and PAN printed on the statement and asks **Whose statement is this?** the first time. After that it recognises the statement by PAN, using a one-way fingerprint; the PAN itself is never stored. Holdings are matched only within the same person, so a fund you both hold stays as two separate holdings.
- **Holdings tab:** with more than one owner, a row of buttons (**Everyone · you · spouse · Joint**) shows each person's total and filters the list. In Edit holdings, each holding has an owner dropdown. **+ Add holdings ▾** offers three ways in: **Enter manually** (a short form), **Import CAS statement (PDF)** and **Upload holdings CSV**. The **⋯ More** button next to it has **Download holdings CSV** (the file to edit in a spreadsheet) and **Guided monthly update**. **Category (optional):** each holding can have a category inside its type, such as *Index funds & ETFs*, *PPF*, *Gold & silver*, or one you create (for example *Property*). Type it in the Category box (setup wizard, Edit holdings, or the Add holding form): pick from the list, or choose **+ New category…** and say what it **counts as** (Equity, Debt, Liquid or Other); picking a category also sets the type. The Holdings list columns are Holding, **Owner** (when more than one family member has holdings), Type, Category, Current value, Invested, Gain, Share and Goal split. What changed since your last snapshot is in the **History** tab (**Since your last snapshot**). In the Holdings list, the **Category** column shows it (grey text is Undiyal's guess when you have not set one), and the Type column shows a **🔒 Locked** badge for money you cannot take out quickly; in Edit holdings, **Can sell quickly** is under Type. Settings → **Categories** lets you rename, re-type or delete your own (deleting keeps the holdings). The four types stay fixed because they drive growth and rebalancing. Without a category, Undiyal guesses one from the name. The CAS import preview has a **Category** column filled with Undiyal's guess (for example *Gold & silver* for gold ETFs and SGBs); change any before importing. The holdings CSV has a **Category** column, filled with your category or Undiyal's guess (as on screen). On upload, a guess left unchanged stays a guess; type a different name to set a category (a new name creates one under that row's type), or empty the cell to remove yours. **List · Split table** switches the view. Tick **Group by type** to show holdings under Equity, Debt, Liquid and Other, each with its count, total and share of savings (inside each type, holdings are sorted by category; a column sort, if you pick one, applies within each category); click a group to collapse or expand it. Click a column heading (Holding, Type, Current value, Gain, Share and so on) to sort: once for one direction, again to reverse, a third time to go back to your own order. Sorting works inside each group. The **Split table** has a Type column too, and its headings sort the same way, including each goal's % column (to see which holdings fund Retirement most) and **Split** (to find holdings that are not fully assigned). The grouping, collapsed groups and sort are remembered in your file. While you edit holdings, the list keeps the order it had on screen (without group headings), so rows do not move as you type; it re-sorts when you click Done. The Goal split column shows the largest goal, for example "Retirement 70% +1 more"; hover or click to see and edit the full split. Enter manually opens a short form. The name box suggests common investments (EPF, VPF, PPF, NPS, Sukanya Samriddhi, SCSS, NSC, KVP, Post Office schemes, FD/RD, SGB, gold, REITs, property and more), or you can type your own. It also has owner, type and liquidity (both guessed from the name, for example EPF is Debt and locked), current value, invested amount and goal. **Save and add another** keeps the form open for the next one. The new holding appears at the top of the list, highlighted, and Undo works.
- **Two PFs or PPFs:** add one holding for each person and set its owner, for example "EPF" (you) and "EPF" (spouse).
- **CSV:** the holdings CSV has an **Owner** column (use the names from About you, or Joint).
- **Reports:** the family summary and the detailed report show totals by person, and the detailed report adds an Owner column.

## Your monthly routine

Use **Guided monthly update** (in the Holdings tab, or from the dashboard reminder). It has three steps:

1. **Statement (CAS):** import this month's CAS. NSDL / CDSL updates shares and mutual funds; CAMS / KFintech updates mutual funds only. The statement is read in your browser.
2. **Other holdings:** type new values for PF, PPF and deposits, or download the holdings CSV, update it in Excel and upload it back. Check each loan's outstanding principal (it is pre-filled from the EMI schedule).
3. **Review and save:** check what changed and save a snapshot.

A **snapshot** records all your values on a date and adds a point to the History chart. Saving again within your reminder period (30 days by default) asks whether to replace the last snapshot or add a new one. The snapshot bar at the top of Holdings appears only when values have changed or a snapshot is due; when everything is up to date it is hidden, and **Guided monthly update** is in the **⋯ More** menu next to Edit holdings.

## The tabs

| Tab | What it is for |
|---|---|
| **Dashboard** | A header with three numbers: **Saved so far**, **Needed by the goal dates** (with the cost in today's prices) and **Invest each month**, a progress bar, and one line on how far today's savings grow on their own (**Show the details** has the rest). Then next steps, KPI cards (total savings, still to cover, net worth), alerts, and the **Goals** section with three views: **Timeline** (each goal as a row with % saved and a dot at its due date on a shared year axis; click a row to open its card), **Cards** (each card shows saved of target, how far your current investments will reach by the goal date, what to invest each month and the Equity : Debt : Liquid : Other mix, with **View details** for the full figures and a **⚖ Rebalance** link when the mix is off) and **Table**; then **Rebalancing by goal**, then five charts that fit together without gaps: **Are we on track?** (saved so far for each goal, with a tick showing where you need to be today), **Portfolio by asset type**, **What's inside your savings** (a ring of equity, debt, liquid and other; point at, tap or tab to a slice to see what is inside it, such as index funds, mid and small cap or shares for equity, or PF, PPF and deposits for debt, then open a group to see its holdings), **Liquidity**, **Savings / Net worth over time** (from your snapshots, once you have 3). Hide a chart with its ✕ button; reorder by dragging its ⠿ handle (computer) or with ↑ ↓ in Settings → Dashboard charts, where you can also turn each one on or off. |
| **Holdings** | Everything you own. Click **Edit holdings** to change values and details (a floating **Done** bar stays at the bottom while you edit), and use **Split table** to assign holdings to goals in an Excel-style grid. **Suggest goal splits** (also on the Assign step of the setup wizard) suggests goal splits by years to each goal and its suggested mix. Names that mention a goal keep it, and EPF/PF/NPS go to retirement. Choose **Only holdings without a goal** (your own splits stay as they are) or **All holdings**, which replaces your current splits and shows them side by side with the suggestion. You see a preview before applying, and Undo works. Import CAS, CSV and the snapshot bar are also here. |
| **Loans** | Home, car, education and personal loans in a read-only table. **Add a loan** and **Edit** open a form where Undiyal calculates the EMI (from amount, rate and tenure), the interest rate (from the EMI), the outstanding principal (from the start date) and the end date and EMIs left; any of these can be changed. The outstanding principal goes down each month on its own; enter your statement's figure to correct it, for example after a prepayment. Also shows **Still to pay** (remaining EMIs, including interest), documents, and totals for outstanding, EMIs and interest. |
| **Goals** | A read-only table of each goal's cost today, target date and years left, inflation and target amount (costs worked out in an earlier year are shown as "₹20 lakh in 2021 money"). Click **Edit goals** to change names, costs, years, inflation, target dates or fixed targets, then **Done**. **Add goal** opens edit mode with the new row. |
| **Corpus** | Retirement corpus calculator. Your age and retirement age come from setup step 1 (and update it if you change them here); for a spouse's retirement goal it uses their ages. Enter expenses and assumptions, including **Money should last until age** (plan above average life expectancy; many planners use 85 to 90), then apply the result to a retirement goal. It shows the corpus at retirement and what that is in today's money. |
| **History** | Your total over time, based on your snapshots, and **Since your last snapshot**: each holding's value then and now, and the change. |
| **Important** | Personal details, ID documents, insurance, bank accounts, deposits, demat accounts, fund folios, property and locker details. Each row can hold attached documents (PDF or images, up to 3 MB each). Sections you have filled in are shown as plain text; click a section's **Edit** button to change it, then **Done**. You can attach documents without editing (Attach / + Add); removing a document is done in Edit. Empty sections open ready to type. A deleted section (including Personal details, Emergency contacts and Where documents are kept) can be added back from **Add a section**, with its usual rows, in its usual place. Custom lists can have their own columns (add, rename or remove them in Edit). **Reorder sections:** on a computer, drag the ⠿ handle next to a section's name (or focus it and press the up and down arrow keys); on a phone, open a section with Edit and use the ↑ ↓ buttons. The order is saved in your data file. |
| **Settings** | Dashboard charts on or off, dashboard alerts, language, text size, theme, number format (lakh/crore or international), expected returns, equity level for long-term goals, reminders, **Categories** (your own ones), and **Your data file** (open another file, save as new file, passphrase, and the date of your last backup). |

## Good to know

- **On a phone,** tables become cards, buttons are larger, and About, text size, theme and downloads are under the ⋯ button at the top.
- **Amounts can be typed with commas** (45,00,000), and the amount appears in words under the field (₹45 lakh).
- **Deleting something shows an Undo** for 10 seconds.
- **Which version you have:** the version (for example 2026.11.13.1) and the data version are shown at the bottom of the start screen and at the top of About. If two computers behave differently, check that both have the same version.
- **About** (top left) opens a short guide in a pop-up, including how to get your CAS. The same guide is in the CAS import box under *How do I get these statements?*
- **Alerts on the dashboard** are coloured by importance, most important first: **red ⚠** needs action now (goal splits that do not add up to 100%, and dates due within 7 days or overdue); **amber ⚠** needs attention soon (a holding over your limit, values not updated, no recent backup, dates 8–30 days away); **blue ℹ** is for your information (a goal cost worked out in an earlier year). Alerts with several items have a **Show details** button. They are grouped:
  - one holding is too large a share of your portfolio;
  - premiums or maturities are due within 30 days;
  - values are out of date;
  - goal splits don't add up to 100%;
  - goal costs are years old;
  - no recent backup.

  You can dismiss most alerts: **Keep this cost** (an old goal cost; it comes back next year or if you change the cost), **Hide until next update** (a large holding; it comes back as soon as any holding value changes), **Done** (each premium, maturity or expiry date; yearly premiums come back next year) and **Remind me later** (out-of-date values or backup; 7 days). Goal-split alerts can only be cleared by fixing the split. **Settings → Dashboard alerts → Show hidden alerts again** brings everything back. Dismissals are saved in your data file.
- **Net worth** is your holdings minus the *outstanding principal* of your loans (not the future interest). Snapshots record loans as well, so History shows net worth over time.
- **Rebalancing** follows a simple rule of thumb: goals ten or more years away can hold more equity, and money moves towards debt as a goal gets closer. Only money you can take out (holdings not marked 🔒 Locked) is suggested for moving; when a goal's money is locked in (PF, PPF, ELSS), Undiyal suggests putting new monthly investments into equity or debt instead. For short-term goals (under 2 years) and emergency or liquid funds, Undiyal shows **Gap to close** (what is still missing and the amount per month, no growth assumed) instead of Monthly needed and Growth needed, and marks the goal **Far behind** when less than half is saved with a year or less to go, or less than a quarter with up to two years to go. It is guidance, not financial advice.
- **Languages:** English, Hindi, Tamil, Telugu and Kannada (Settings → Language). Everything Undiyal writes is translated: tabs, buttons, help text, alerts, next steps, guided tours, About, messages, and the family summary and detailed report. What you type yourself (goal names, fund names, notes) stays as you typed it. The start screen opens in the language you used last. The translations have not yet been checked by native speakers, so some wording may read unnaturally.
- **Accessibility:**
  - text size (A / A+ / A++ in the header);
  - full keyboard use, with tooltips appearing on focus;
  - screen-reader labels on every field;
  - colour-blind-safe chart colours;
  - support for your system's reduced-motion setting.

## Supported statements and files

### Getting your CAS

- **NSDL / CDSL CAS:** arrives by email automatically, at the email registered with your demat account. It comes every month if there were transactions, otherwise every six months. The password is usually your PAN in capital letters.
- **CAMS / KFintech CAS:** request it on camsonline.com (the "CAS – CAMS + KFintech" statement); mfs.kfintech.com and MF Central offer the same.
  1. Choose the detailed statement and the period.
  2. Enter your PAN and the email registered with your funds.
  3. Set a password.

  The PDF arrives by email within a few minutes.

- **CAS:** two kinds, recognised automatically:
  - **NSDL / CDSL CAS** (depository statement): shares, ETFs, bonds and mutual funds. Use this one if you hold shares. Its password is usually your PAN in capital letters.
  - **CAMS / KFintech / MF Central CAS:** mutual funds only (detailed or summary). Its password is the one you set when requesting it.

  **Folio numbers** in the statement are saved to Important → Mutual fund folios (with the fund house), not shown in Holdings, and listed in the family summary. Untick the option in the import preview to skip this. The **statement PDF itself** is kept in Important → Account statements (CAS), one per statement type (NSDL / CDSL and CAMS / KFintech); importing a newer one replaces the older PDF. It stays password-protected, and PDFs over 3 MB are not stored. It is saved only when the import succeeds (at least one holding imported). To skip it, untick *Keep this statement…* under the password field or on the import preview; your choice is saved in your data file. Both password-protected and AES-256 encrypted PDFs are supported. Holdings that appear in both statements are matched by ISIN, so they are not counted twice.
- **CSV:** use **Download holdings CSV** (in **⋯ More**) to get the right columns: ID, Holding, Owner, Type, Category, Liquid, Current value, Invested and one "% column" per goal. Keep the ID column as it is, and leave it empty for new holdings. Upload it back with **+ Add holdings ▾ → Upload holdings CSV**; you see every change before it is applied.

## Troubleshooting

- **"Saving files is not available" or a download every time:** your browser cannot write to files (Firefox, Safari or an older phone browser). Use Save data and replace your old file with the newest download, or use Chrome or Edge on a computer, or Chrome on Android.
- **The CAS shows no holdings:** check that it is an NSDL / CDSL, CAMS, KFintech or MF Central CAS and that the password is right, then use **Show extracted text** to see what was read.
- **A fund name looks cut short:** re-import the CAS. If it is still short, edit it in Holdings → Edit holdings.
- **Blank page or "Undiyal can't run here" on iPhone or iPad:** iPhone and iPad are not supported. Use a computer or an Android phone.
- **The file won't open:** if it was encrypted, check the passphrase. Otherwise, try your latest backup.

## Disclaimer

- **Not financial advice:** Undiyal is a personal tracking tool. It does not give investment, tax or financial advice, and its creator is not a SEBI-registered investment adviser. Speak to a qualified adviser before making financial decisions.
- **Estimates only:** Targets, retirement corpus, monthly investment, rebalancing suggestions and loan figures are estimates based on your own assumptions (returns, inflation, interest rates). Actual results will differ. Past returns do not guarantee future returns.
- **Check your figures:** Values come from what you enter and from statements Undiyal reads (CAS, CSV). Reading may be incomplete or wrong, so always check against your official statements. Loan balances are projections; your lender’s statement is final.
- **Before tax and charges:** Figures do not deduct capital gains tax, TDS, exit loads or other charges.
- **Your data, your responsibility:** Your information stays only in your file on your device; nothing is collected or uploaded. Keep backup copies. If you forget your passphrase, the file cannot be recovered. Family summaries contain your financial details, so share them with care.
- **No affiliation:** CAMS, KFintech, MF Central, NSDL, CDSL and other names belong to their owners. Undiyal is not affiliated with or endorsed by them.
- **No warranty:** Undiyal is provided as is, without warranty of any kind. Its creator is not liable for any loss arising from its use.

## Licence

© 2026 The Undiyal authors. Released under the [MIT License](LICENSE): free to use, share and modify, provided as is without warranty.

## Files in this folder

| File | Purpose |
|---|---|
| `Undiyal.html` | Undiyal itself. Open this file. |
| `undiyal-data.json` | Your data (older files may be called `investment-data.json`). |
| `README.md` | This guide. |
| `LICENSE` | MIT licence. Share it together with `Undiyal.html`. |

## Opening files from older or newer versions

- Every data file records a **data version** (shown in About and on the start screen, next to the app version).
- **Older file:** Undiyal shows an **Updating your data file** screen before opening it, and runs four checked steps: (1) **save a copy of the original**, untouched and still encrypted if it was (`undiyal-before-update-YYYY-MM-DD.json`, in your downloads); (2) **update the data** on a copy in memory; (3) **check that nothing was lost**: the number of holdings, goals, snapshots and record sections and the total value must be the same, and the screen shows them; (4) **check that the updated file saves and opens** (for a protected file, it is encrypted and decrypted again). Each step gets a tick. If any step fails, Undiyal stops, says which step, and opens nothing; your original file is not changed. Click **Open my data** when all four have passed.
- **Newer file** (saved by a newer Undiyal): you can **Open read-only** to look at it. Nothing is saved; download the latest `Undiyal.html` to edit it.
