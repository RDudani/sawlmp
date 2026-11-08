# sawlmp.com - Static Website for GitHub Pages

This is the production static website for **sawlmp.com**, restored and optimized for **$0/month hosting** on **GitHub Pages** with custom **GoDaddy DNS** mapping.

---

## 🚀 How to Put This in Your GitHub Repository

### Option A: Web Browser (Zero Terminal / No Git Needed)
1. Go to [github.com/new](https://github.com/new) and create a repository named **sawlmp-website** (Set it to **Public**).
2. Click **"uploading an existing file"**.
3. Drag and drop all the files from this folder (`index.html`, `CNAME`, `.nojekyll`, `README.md`).
4. Click **"Commit changes"**.
5. In your repository, go to **Settings** → **Pages**:
   - Under **Build and deployment → Branch**, choose `main` and folder `/ (root)`, then click **Save**.
   - Under **Custom domain**, enter `sawlmp.com` and click **Save**.
   - Check **Enforce HTTPS** once DNS checks complete.

---

### Option B: Using Git in Terminal
```bash
# Initialize and push to your GitHub repo
git init
git add .
git commit -m "Deploy static website for sawlmp.com"
git branch -M main
git remote add origin https://github.com/rohitdudani/sawlmp-website.git
git push -u origin main
```

---

## 🌐 GoDaddy DNS Configuration

In your **GoDaddy Domain Portfolio** → Click **sawlmp.com** → **Manage DNS**:

| Type | Name | Value / Points To | TTL |
| :--- | :--- | :--- | :--- |
| **A** | `@` | `185.199.108.153` | 1/2 Hour (600s) |
| **A** | `@` | `185.199.109.153` | 1/2 Hour (600s) |
| **A** | `@` | `185.199.110.153` | 1/2 Hour (600s) |
| **A** | `@` | `185.199.111.153` | 1/2 Hour (600s) |
| **CNAME** | `www` | `rohitdudani.github.io` | 1/2 Hour (1800s) |

> ⚠️ **Important:** In GoDaddy, make sure to delete any existing default "Parked" A record before adding the 4 A records above.
