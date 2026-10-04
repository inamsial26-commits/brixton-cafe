# BRIXTON CAFE & RESTAURANT - Official Web Application

Modern, high-conversion React + Vite web application for **BRIXTON CAFE & RESTAURANT** (Qadirpur Ran, Multan). Features interactive online ordering, direct WhatsApp checkout, Google Maps directions, dynamic menu categories, and a bulletproof image fallback architecture.

---

## 🚀 Free Deployment on Vercel with GitHub Integration

### Step 1: Push Code to GitHub
1. Create a new repository on [GitHub](https://github.com/new) named `brixton-cafe-restaurant` (keep it Public or Private).
2. Initialize and push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Brixton Cafe & Restaurant"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/brixton-cafe-restaurant.git
   git push -u origin main
   ```

### Step 2: Connect GitHub to Vercel (100% Free Hobby Tier)
1. Sign in or create a free account at [Vercel](https://vercel.com) using your **GitHub account**.
2. Click **"Add New..."** → **"Project"**.
3. Under **"Import Git Repository"**, locate `brixton-cafe-restaurant` and click **"Import"**.

### Step 3: Verify Build Settings
Vercel automatically detects the preset from `vercel.json`:
- **Framework Preset**: `Vite`
- **Root Directory**: `./`
- **Build Command**: `npm run build`
- **Output Directory**: `dist`
- **Install Command**: `npm install`

Click **"Deploy"**. Within ~30 seconds, your site is live with a secure `https://*.vercel.app` domain and free global CDN!

### Step 4: Continuous Deployment (CI/CD)
Whenever you push changes to your `main` branch on GitHub:
```bash
git add .
git commit -m "Update menu prices and items"
git push origin main
```
Vercel will automatically build and deploy the update with zero downtime.

---

## 🛠️ Local Development

```bash
# 1. Install dependencies
npm install

# 2. Run local dev server
npm run dev

# 3. Build for production
npm run build

# 4. Preview production build
npm run preview
```

---

## 📁 Key File Structure

- `src/data/restaurantData.ts` - Centralized restaurant info, WhatsApp link, and `DEMO_IMAGES` catalog
- `src/components/SafeImage.tsx` - Zero-blank image component with multi-level fallbacks & inline SVG failsafe
- `vercel.json` - SPA routing rewrites configuration for Vercel
