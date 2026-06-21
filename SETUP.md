# Setup — getting your Command Centre page live

This takes about 10 minutes and needs no coding. You're putting this folder onto
GitHub (free) and switching on its built-in website feature (GitHub Pages).

The result:
- A **live download page** at `https://<your-username>.github.io/founder-command-centre/`
- A **plugin library** people can add inside Claude for one-click install + auto-updates

---

## Step 1 — Create the repository

1. Go to **github.com** and sign in (or create a free account).
2. Click **New repository**.
3. Name it **`founder-command-centre`** (this name becomes part of your web address).
4. Set it to **Public** (required for the free website + for others to install).
5. Click **Create repository**.

## Step 2 — Upload these files

1. On the new repo page, click **uploading an existing file**.
2. Drag in **everything inside the `founder-command-centre-site` folder** — including
   the hidden `.claude-plugin` and `ai-herway-founder-command-centre` folders.
   (If drag-and-drop hides the dotted folders, use **Add file → Upload files** and
   select all, or use GitHub Desktop.)
3. Click **Commit changes**.

## Step 3 — Turn on the website (GitHub Pages)

1. In the repo, go to **Settings → Pages**.
2. Under **Source**, choose **Deploy from a branch**.
3. Branch: **main**, folder: **/(root)**. Click **Save**.
4. Wait 1–2 minutes. Your page goes live at:
   **`https://<your-username>.github.io/founder-command-centre/`**

That URL is your shareable download page. The marketplace source instructions on the
page fill in your repo automatically once it's hosted — nothing to edit.

## Step 4 — (Optional) put it on your own domain

To use something like **`commandcentre.aiherway.com`** instead of the github.io address:

1. In your domain/DNS settings, add a **CNAME** record pointing your chosen subdomain
   to `<your-username>.github.io`.
2. In the repo's **Settings → Pages → Custom domain**, enter that subdomain and save.

(If you'd rather keep it on your main site, you can also just upload `index.html` and
`ai-herway-founder-command-centre.plugin` to your existing website host — but you'd
lose the auto-updating library feature, which only the GitHub route gives you.)

## Step 5 — For the retreat (Thursday)

The fastest path for the room: share the live page link, or point the deck's QR code
at it. Each woman taps **Download the plugin**, opens it in Claude, presses **Add**.
The copy-paste fallback (in the Noosa folder) covers anyone who can't install.

---

## How updates work later

When we add or improve a skill, update the files in this repo and bump the version in
`ai-herway-founder-command-centre/.claude-plugin/plugin.json` and
`.claude-plugin/marketplace.json`. Anyone who installed via the **library** (method 2)
gets the update automatically. Anyone who used the **download** (method 1) just grabs
the file again.

This is the structure that lets the Command Centre sit behind Nikki's SuperLeaders
platform later — same library, with the agents offered as add-ons.

---
© AI Her Way · Dr Nici Sweaney · aiherway.com.au
