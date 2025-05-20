# Deployment Guide: Publishing Your CV Website

## GitHub Pages (Recommended)

GitHub Pages is an excellent free hosting solution for static websites like your CV page. Here's how to deploy your site:

### Step 1: Create a GitHub Account

If you don't already have one, sign up at [GitHub](https://github.com/signup).

### Step 2: Create a New Repository

1. Click the '+' icon in the top right corner and select 'New repository'
2. Name your repository (e.g., `my-cv` or `portfolio`)
3. Make it public
4. Click 'Create repository'

### Step 3: Upload Your Files

**Option A: Using GitHub Web Interface**

1. In your new repository, click 'uploading an existing file'
2. Drag and drop all your website files and folders
3. Commit the changes

**Option B: Using Git Command Line**

```bash
# Navigate to your project folder
cd "/Users/alanfried/cv page"

# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit"

# Add the remote repository (replace USERNAME with your GitHub username and REPO with your repository name)
git remote add origin https://github.com/USERNAME/REPO.git

# Push to GitHub
git push -u origin main
```

### Step 4: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click 'Settings'
3. Scroll down to 'GitHub Pages' section
4. Under 'Source', select 'main' branch
5. Click 'Save'

Your site will be published at `https://USERNAME.github.io/REPO/` (replace USERNAME with your GitHub username and REPO with your repository name).

## Alternative Free Hosting Options

### Netlify

1. Sign up at [Netlify](https://www.netlify.com/)
2. Click 'New site from Git'
3. Connect to your GitHub repository
4. Deploy your site

Benefits: Custom domain support, HTTPS, continuous deployment, and form handling.

### Vercel

1. Sign up at [Vercel](https://vercel.com/)
2. Import your GitHub repository
3. Deploy your site

Benefits: Excellent performance, global CDN, and preview deployments.

### Render

1. Sign up at [Render](https://render.com/)
2. Create a new 'Static Site'
3. Connect to your GitHub repository
4. Deploy your site

Benefits: Free SSL, global CDN, and continuous deployment.

## Custom Domain (Optional)

If you want to use a custom domain (e.g., alanfried.com):

1. Purchase a domain from a registrar like Namecheap, GoDaddy, or Google Domains
2. Follow the hosting provider's instructions to connect your custom domain

All the hosting options mentioned above support custom domains on their free plans.

## Updating Your Website

To update your website after deployment:

1. Make changes to your local files
2. Commit and push the changes to GitHub
3. Your hosting provider will automatically rebuild and deploy your site

```bash
git add .
git commit -m "Update website content"
git push
```

## Troubleshooting

If your site doesn't appear after deployment:

1. Check if the repository is public
2. Ensure the correct branch is selected in GitHub Pages settings
3. Verify that index.html is in the root directory
4. Wait a few minutes for the deployment to complete

For more help, refer to [GitHub Pages documentation](https://docs.github.com/en/pages).