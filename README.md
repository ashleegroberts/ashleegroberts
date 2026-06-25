# ashleegroberts.com — Site Files

Plain HTML and CSS. No frameworks, no build tools needed.

---

## File Structure

```
ashleegroberts-site/
├── index.html
├── css/
│   └── main.css
├── pages/
│   ├── about.html
│   ├── digital-products.html
│   ├── green-star-grove.html
│   ├── shop.html
│   └── disclosure.html
├── images/          ← add your photos here
└── .github/
    └── workflows/
        └── deploy.yml   ← do not touch, GitHub reads this to deploy
```

---

## How to Upload to GitHub

1. Go to github.com and open your repository
2. Click **Upload files**
3. Drag everything from this unzipped folder into the upload area
4. Keep the folder structure exactly as-is
5. Scroll down, write "updated site files" and click **Commit changes**
6. GitHub deploys automatically within 2 to 3 minutes

---

## Enable GitHub Pages (first time only)

1. In your repo, go to **Settings → Pages**
2. Under Source, select **GitHub Actions**
3. Save — that is it

---

## Connect ashleegroberts.com (if not done yet)

1. Settings → Pages → Custom Domain → type ashleegroberts.com → Save
2. In Namecheap → Advanced DNS, add:
   - Type: CNAME
   - Host: www
   - Value: yourusername.github.io
3. Also add four A records pointing to GitHub's IPs:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153
4. Wait 15 to 30 minutes for DNS to propagate

---

## Swapping Placeholders Before You Publish

Search all files for these and replace:

| Placeholder | Replace with |
|---|---|
| YOUR_KIT_FREEBIE_LINK | Your Kit freebie landing page URL |
| YOUR_KIT_PRODUCT_LINK_HERE | Your Kit product page URL |
| YOUR_NEWBORN_LIST_ID | Amazon Idea List ID for newborn products |
| YOUR_2MO_LIST_ID | Amazon Idea List ID for 2-month products |
| YOUR_4MO_LIST_ID | Amazon Idea List ID for 4-month products |
| YOUR_6MO_LIST_ID | Amazon Idea List ID for 6-month products |
| YOUR_9MO_LIST_ID | Amazon Idea List ID for 9-month products |

---

## Adding Photos

Add image files to the images/ folder, then replace placeholder emoji divs with:
```html
<img src="../images/your-photo.jpg" alt="description">
```
Use ../images/ from inside pages/ folder, or images/ from index.html.

---

## Editing Content

Open any .html file in a text editor, find the text, change it, save, re-upload to GitHub. Changes go live in 2 to 3 minutes after upload.

To change colors, open css/main.css and edit values under :root { } at the top.
