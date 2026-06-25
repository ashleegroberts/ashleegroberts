# ashleegroberts.com — Site Files

Built with plain HTML and CSS. No frameworks, no build tools, no terminal commands needed beyond the initial GitLab setup.

---

## File Structure

```
ashleegroberts-site/
├── index.html              ← Home page
├── css/
│   └── main.css            ← All styles — edit colors and fonts here
├── pages/
│   ├── about.html
│   ├── digital-products.html
│   ├── green-star-grove.html
│   ├── shop.html
│   ├── disclosure.html
│   └── privacy.html        ← Add this when ready
├── images/                 ← Add your photos here
│   └── (your images go here)
└── .gitlab-ci.yml          ← Do not touch — GitLab reads this to deploy
```

---

## How to Set Up on GitLab Pages (Step by Step)

### First-time setup

1. Go to gitlab.com and create a free account if you don't have one
2. Click **New Project → Create blank project**
3. Name it exactly: `ashleegroberts` (lowercase, no spaces)
4. Set visibility to **Public**
5. Click **Create project**

### Upload your files

**Option A — Drag and drop (easiest)**
1. Inside your new project, click the **+** button → **Upload file**
2. Drag all the files from this folder into the upload area
3. Keep the folder structure exactly as-is (css/ folder, pages/ folder, etc.)
4. Click **Commit changes**

**Option B — GitLab Web IDE**
1. Inside your project, press the `.` key on your keyboard — this opens the Web IDE
2. Drag and drop your files into the file tree on the left
3. Click **Commit** when done

### Connect your domain (ashleegroberts.com)

1. In your GitLab project, go to **Settings → Pages**
2. Click **New Domain**
3. Enter: `ashleegroberts.com`
4. GitLab gives you a DNS record to add — copy it
5. Log into Namecheap → select ashleegroberts.com → **Advanced DNS**
6. Add the record GitLab gave you (usually a CNAME or TXT record)
7. Wait 15 to 30 minutes for DNS to propagate
8. Your site will be live at ashleegroberts.com

---

## Before You Publish — Swap These Placeholders

Search all files for these strings and replace them:

| Placeholder | Replace with |
|---|---|
| `YOUR_KIT_FREEBIE_LINK` | Your Kit freebie landing page URL |
| `YOUR_KIT_PRODUCT_LINK_HERE` | Your Kit product page URL for the guide |
| `YOUR_NEWBORN_LIST_ID` | Your Amazon Idea List ID for newborn products |
| `YOUR_2MO_LIST_ID` | Your Amazon Idea List ID for 2-month products |
| `YOUR_4MO_LIST_ID` | Your Amazon Idea List ID for 4-month products |
| `YOUR_6MO_LIST_ID` | Your Amazon Idea List ID for 6-month products |
| `YOUR_9MO_LIST_ID` | Your Amazon Idea List ID for 9-month products |

To find your Amazon Idea List ID:
1. Go to amazon.com and create a new Idea List for each phase
2. Add your recommended products to each list
3. Click Share — the URL contains your list ID (it looks like `3ABCDEF123456`)

---

## How to Add Your Photos

1. Add your photo files to the `images/` folder
2. In any HTML file, replace the placeholder emoji divs with:
   ```html
   <img src="../images/your-photo-name.jpg" alt="Description of photo">
   ```
   (Use `../images/` from inside the pages/ folder, or just `images/` from index.html)

---

## How to Edit Content

Every page is just an HTML file. To change text:
1. Open the file in the GitLab Web IDE (press `.` in your project)
2. Find the text you want to change
3. Edit it directly
4. Click Commit — changes go live in about 2 minutes

To change colors, open `css/main.css` and edit the values under `:root { }` at the top.

---

## Questions?

Email ashleegroberts@gmail.com or ask Claude — just paste in the file you want to change.
