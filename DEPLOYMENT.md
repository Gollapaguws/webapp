# Deploy to GitHub Pages (Automatic SSL)

This site is configured for GitHub Pages deployment with automatic SSL/HTTPS.

## Automatic Deployment

GitHub Pages will automatically serve your site over HTTPS at:
`https://gollapaguws.github.io/webapp/`

## Enable GitHub Pages

1. Go to your repository: https://github.com/Gollapaguws/webapp
2. Click **Settings** → **Pages**
3. Under **Source**, select branch: `main` and folder: `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for deployment
6. Your site will be available at: `https://gollapaguws.github.io/webapp/`

GitHub automatically provides free SSL certificates via Let's Encrypt.

## Custom Domain with SSL (Optional)

If you want to use a custom domain:

1. Add a `CNAME` file with your domain name
2. Configure DNS with your domain provider:
   - Add A records pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add CNAME record: `gollapaguws.github.io`
3. In GitHub Pages settings, add your custom domain
4. Check "Enforce HTTPS" (available after DNS propagation)

## Alternative: Deploy to Netlify/Vercel (One Command)

Both platforms provide automatic SSL and are free for static sites.

### Netlify
```powershell
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod
```

### Vercel
```powershell
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel --prod
```

Both will give you a `https://` URL immediately with automatic SSL.
