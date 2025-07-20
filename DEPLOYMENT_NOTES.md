# 4-Wave Labs Deployment Notes

## Project Overview
- **Website**: 4wavelabs.com
- **Platform**: Vercel
- **Project Type**: Static HTML website
- **Framework**: Static files (HTML/CSS)

## Deployment Setup
- **Vercel Account**: watsys-projects
- **Project Name**: 4wavelabs
- **Custom Domain**: 4wavelabs.com

## How to Deploy Updates

### Method 1: Using Vercel CLI (Recommended)
```bash
# Navigate to project directory
cd c:\Users\PC\CascadeProjects\4wavelabs

# Deploy to production
vercel --prod
```

### Method 2: Using Windsurf Deploy Tool
- Use the deploy_web_app tool with framework "jekyll"
- This creates a new deployment, not recommended for existing sites

## Important Files
- `index.html` - Main homepage
- `contact.html` - Contact page
- `.vercel/` - Vercel configuration (DO NOT DELETE)
- `netlify.toml` - Configuration file (can be ignored for Vercel)
- `.gitignore` - Git ignore file

## Vercel CLI Commands
```bash
# Check deployments
vercel ls

# Check current status
vercel --version

# Deploy to production
vercel --prod

# Deploy to preview
vercel
```

## Troubleshooting

### If custom domain isn't updating:
1. Check if deployment was successful: `vercel ls`
2. Wait 5-10 minutes for CDN cache to clear
3. Try hard refresh (Ctrl+F5) on browser

### If you get authentication errors:
1. Login to Vercel: `vercel login`
2. Follow the authentication prompts

### If deployment fails:
1. Check if you're in the correct directory
2. Ensure `.vercel` folder exists
3. Try `vercel --prod --force` to force redeploy

## Project Structure
```
4wavelabs/
├── index.html          # Main page
├── contact.html        # Contact page
├── .vercel/           # Vercel config (auto-generated)
├── .gitignore         # Git ignore
├── netlify.toml       # Config file (not used for Vercel)
└── DEPLOYMENT_NOTES.md # This file
```

## Last Successful Deployment
- **Date**: 2025-07-06 04:02 ACST
- **URL**: https://4wavelabs-92a0zl5kp-watsys-projects.vercel.app
- **Status**: ✅ Ready (Production)
- **Build Time**: 2 seconds

## Contact Information on Site
- **Email**: watsy@4wavelabs.com
- **Description**: Advanced Search Technology with 4-Wave Algorithm

## Notes for Future Updates
1. Always use `vercel --prod` for production deployments
2. The `.vercel` folder contains your project configuration - don't delete it
3. Changes should appear on 4wavelabs.com within 5-10 minutes
4. If you need to make quick edits, edit the HTML files directly and redeploy
5. For major changes, test locally first if needed

## Emergency Contacts
- Vercel Dashboard: https://vercel.com/dashboard
- Project URL: https://vercel.com/watsys-projects/4wavelabs

---
*Last updated: 2025-07-06*
