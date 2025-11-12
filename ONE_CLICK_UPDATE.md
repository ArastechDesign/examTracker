# 🚀 One-Click Update to v1.0.1

Update your existing Exam Tracker deployment to v1.0.1 with **one click**!

## ✨ What's New in v1.0.1

- 🌍 **Dual-language support** (English ↔ Malay)
- 🎨 **Enhanced admin interface** with modal editor
- ⚡ **Quick add buttons** for rapid exam creation
- 📥 **Bulk import/export** functionality
- 🔧 **Improved form validation** and UX
- 💡 **Help tooltips** and better error messages

## Step 1: Find Your KV Namespace ID

1. Go to https://dash.cloudflare.com/
2. Click **Workers & Pages** → **KV**
3. Find your namespace (usually ends with `EXAM_DATA`)
4. Click on it and copy the **Namespace ID**
   - It looks like: `abc123def456ghi789jkl012`

**Can't find it?** Check under **Workers** → Your Worker → **Settings** → **Variables** → **KV Namespace Bindings**

## Step 2: Update via GitHub Actions

1. Go to your **forked repository** on GitHub
2. Click the **Actions** tab
3. Click **Update to Latest Version** workflow
4. Click **Run workflow**
5. Fill in the details:
   - **Worker Name**: Your existing worker name (e.g., `spm-2025`, `finals-tracker`)
   - **KV Namespace ID**: Paste the ID you copied
6. Click **Run workflow**

## Step 3: Wait & Enjoy!

The update takes about **1 minute**. You'll get a notification when it's done.

## ✅ What Gets Preserved

- **All your exam data** - Nothing is lost!
- **Your custom worker name** - Same URL
- **Admin password** - Unchanged
- **Configuration** - Title, description, settings

## 🎯 Your Updated Features

After updating, you'll have:

**🌐 Public Interface:**
- Language switcher button (EN/BM) in top-right
- All text translates instantly

**🔐 Admin Panel:**
- Modal-based exam editor (much better UX!)
- Quick add buttons (Today/Tomorrow/This Week)
- Bulk import/export with JSON
- Free-text categories
- Help tooltips on form fields

## Troubleshooting

**"KV namespace not found"**
- Double-check your Namespace ID is correct
- Make sure you're using the ID from your Cloudflare dashboard

**"Unauthorized"**
- Verify your `CLOUDFLARE_API_TOKEN` secret is still valid in GitHub

**"Worker not found"**
- Make sure the worker name matches exactly (case-sensitive)

## Need Help?

- Check the **Actions** logs for detailed error messages
- Open an issue on GitHub with the error details
- Your data is safe - updates are non-destructive!

---

**🎉 Happy updating! Your exam tracker just got a major upgrade.**