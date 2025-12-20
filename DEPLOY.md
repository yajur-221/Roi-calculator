# Deploy ROI Calculator

## Option 1: GitHub Pages (Recommended)

### Steps:
1. Go to https://github.com/new and create a new repository named `thehirehub-roi-calculator`
2. Run these commands in your terminal:

```bash
cd /Users/yajursmac/thehirehub-roi-calculator
git remote add origin https://github.com/YOUR_USERNAME/thehirehub-roi-calculator.git
git branch -M main
git push -u origin main
```

3. Go to your repository on GitHub → Settings → Pages
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click "Save"
7. Your calculator will be live at: `https://YOUR_USERNAME.github.io/thehirehub-roi-calculator/roi-calculator.html`

## Option 2: Netlify Drop (Easiest - No account needed)

1. Go to https://app.netlify.com/drop
2. Drag and drop the `roi-calculator.html` file
3. You'll get an instant live link!

## Option 3: Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel` in the project directory
3. Follow the prompts
4. Your site will be live instantly!

