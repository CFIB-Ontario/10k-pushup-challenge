# Deploying to Vercel

This guide will help you deploy your 10K Pushup Tracker to Vercel for free hosting.

## Prerequisites
- GitHub account (you already have this!)
- Vercel account (free - sign up with your GitHub account)

## Step 1: Upload Files to GitHub

1. Go to your GitHub repository (the one you created)
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop ALL these files:
   - `index.html`
   - `favicon.svg`
   - `vercel.json`
   - `README.md`
4. Scroll down and click **"Commit changes"**

## Step 2: Make Repository Public (Required for Free Vercel)

1. Go to your repository **Settings**
2. Scroll to **"Danger Zone"**
3. Click **"Change visibility"**
4. Select **"Make public"**
5. Confirm by typing the repository name

## Step 3: Deploy to Vercel

### Option A: Using Vercel Dashboard (Easiest)

1. Go to **https://vercel.com**
2. Click **"Sign Up"** (or "Log In" if you have an account)
3. Choose **"Continue with GitHub"**
4. Authorize Vercel to access your GitHub
5. Click **"Import Project"** or **"Add New..."** → **"Project"**
6. Find your `pushup-tracker` repository
7. Click **"Import"**
8. Vercel will auto-detect settings (no changes needed)
9. Click **"Deploy"**
10. Wait ~30 seconds for deployment
11. Done! You'll get a URL like: `https://pushup-tracker-xyz.vercel.app`

### Option B: Using Vercel CLI (Advanced)

```bash
# Install Vercel CLI
npm install -g vercel

# Navigate to your project folder
cd pushup-tracker

# Deploy
vercel

# Follow the prompts
```

## Step 4: Access Your App

After deployment completes:
- Vercel gives you a URL like: `https://your-project.vercel.app`
- Bookmark this URL on your phone/computer
- Your app is now live and accessible from anywhere!

## Features After Deployment

✅ **Always online** - Access from any device
✅ **HTTPS** - Secure connection
✅ **Fast loading** - Vercel's global CDN
✅ **Free** - No cost for this simple app
✅ **Auto-updates** - Push to GitHub, Vercel auto-deploys

## Custom Domain (Optional)

Want `pushups.yourname.com`?

1. Buy a domain (Namecheap, Google Domains, etc.)
2. Go to Vercel Dashboard → Your Project → **Settings** → **Domains**
3. Add your custom domain
4. Follow DNS configuration instructions
5. Done!

## Updating Your App

After initial deployment:
1. Make changes to your files
2. Upload to GitHub (same way as before)
3. Vercel **automatically redeploys** in ~30 seconds
4. No extra steps needed!

## Troubleshooting

**"Build failed"**: Make sure all files are uploaded and `index.html` is in the root folder

**"Can't find repository"**: Make sure the repository is public

**"404 Not Found"**: Check that `index.html` is in the root (not in a subfolder)

## Privacy Note

Even though the repository is public:
- Your **pushup data** stays private (it's stored in your browser only)
- The public repository just contains the app code
- No one can see your personal workout data

---

**Questions?** The Vercel docs are excellent: https://vercel.com/docs

**Ready to deploy!** 🚀💪
