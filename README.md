# AJIBOYE OLUWASEYI | Software Developer Portfolio

A professional, production-ready portfolio website built with pure HTML, CSS (Tailwind), and JavaScript. Zero backend required.

## ✨ Features

- **Fully Static** - No backend server needed
- **Mobile Responsive** - Works on all devices
- **Dark Mode** - System preference detection + manual toggle
- **Serverless Forms** - Netlify Forms handles contact submissions
- **GitHub Integration** - Auto-loads your projects from GitHub
- **PDF Resume** - Direct download & view functionality
- **SEO Optimized** - Meta tags, semantic HTML
- **Performance** - Fast loading, optimized assets
- **Professional Gradient** - Beautiful hero section with premium UI

## 🚀 Quick Setup

### 1. Local Development

```bash
npm install
npm run dev
```

Opens at `http://localhost:3000`

### 2. Personalization

**Update your profile:**

- Edit name, bio in `index.html` lines 66-90
- Replace profile image: `./images/Snapchat-1252159438.jpg`
- Update GitHub username: Line 941 `const githubUsername = "ajiboy-dev"`
- Update social links in footer: Lines 930-936

**Add your CV:**

- Place your PDF in root folder and name it `Ajiboye_Oluwaseyi_CV.pdf`
- The CV section (line 558) already links to this file
- View and download buttons will work once deployed

## 📋 How Your GitHub Projects Load

The portfolio automatically fetches your GitHub repositories:

1. Your GitHub username is set to `ajiboy-dev`
2. On page load, it queries the GitHub API: `https://api.github.com/users/ajiboy-dev/repos`
3. Filters out forks and displays your top 6 repos (by update time)
4. For each repo, it shows:
   - Name & description (from GitHub)
   - Language (from GitHub)
   - Links to code and homepage (if set)

**To add project details:**

- Add descriptions to your GitHub repos
- Set a homepage URL in repo settings for "Live Demo" buttons
- Repos will update automatically when deployed

## ✅ No Backend Required

This is a **fully static portfolio**:

- ✅ HTML + CSS (Tailwind) + JavaScript only
- ✅ Contact form handled by Netlify Forms (serverless)
- ✅ GitHub API fetches projects (read-only)
- ✅ Form submissions redirect to `thanks.html`
- ✅ Zero server maintenance needed

## 🌐 Deployment Guide

### Option 1: Netlify (Recommended) ✨

1. **Create account:** https://netlify.com
2. **Connect repository:**
   - Click "Add new site" → "Import an existing project"
   - Connect your GitHub repo
   - Base directory: `new-portfolio`
   - Deploy!
3. **Enable Netlify Forms:**
   - Go to Site settings → Forms
   - Forms are auto-detected and enabled
4. **Custom Domain:**
   - Settings → Domain management → Add custom domain

**Result:** Your contact form will capture submissions, CV download works, GitHub projects auto-load.

### Option 2: Vercel

1. Create account: https://vercel.com
2. Click "New Project" → Import your repo
3. Root directory: `new-portfolio`
4. Deploy!

**Note:** Contact form won't work on Vercel (it uses Netlify Forms). You'd need to use Vercel's form integration or switch to Netlify.

### Option 3: GitHub Pages

1. Push code to GitHub
2. Go to Settings → Pages
3. Set source to `main` branch, folder `/new-portfolio`
4. GitHub will provide your live URL

**Note:** GitHub Pages won't handle contact form submissions.

## 📝 Resume/CV Section

**Why your resume might not be showing:**

✅ **Fixed in this update:**

- Added complete CV section with View & Download buttons
- Links to `Ajiboye_Oluwaseyi_CV.pdf` (your current file)
- Works on all domains (Netlify, Vercel, local)

**To enable:**

1. Your file `Ajiboye_Oluwaseyi_CV.pdf` is already in the root folder ✓
2. CV section is now in the HTML (line 558) ✓
3. When deployed, users can click "View CV" or "Download CV"
4. On local: Use `npm run dev` to test the links

## 🎨 What I Changed

### 1. Hero Section Gradient

- **Before:** `from-slate-900 via-slate-800 to-primary/80` (gray)
- **After:** `from-indigo-600 via-purple-500 to-pink-500` (vibrant professional gradient)
- Button styles updated to white with shadow
- Text now white for contrast on colorful background

### 2. CV Section Added

- New section between projects and testimonials
- Direct link to `Ajiboye_Oluwaseyi_CV.pdf`
- View & Download buttons
- Mobile responsive
- Dark mode support

### 3. Enhanced netlify.toml

- Added build command
- PDF caching headers
- Image optimization headers
- Security headers (X-Content-Type-Options, etc.)
- SPA routing redirect
- Proper framework detection

## 📋 Pre-Deployment Checklist

- [ ] Updated name & bio in HTML
- [ ] Replaced profile image with your photo
- [ ] Added GitHub username
- [ ] CV file `Ajiboye_Oluwaseyi_CV.pdf` is in root folder
- [ ] Updated social links (GitHub, LinkedIn, portfolio)
- [ ] Tested locally with `npm run dev`
- [ ] Verified CV downloads/views locally
- [ ] Updated project descriptions on GitHub
- [ ] Added homepage URLs to repos (for live demo links)

## 🔗 Production URLs

Once deployed, your portfolio will be accessible at:

- **Netlify:** `your-name.netlify.app`
- **Vercel:** `your-name.vercel.app`
- **GitHub Pages:** `username.github.io` or `username.github.io/new-portfolio`
- **Custom Domain:** Your own domain (configure in hosting provider)

## 📧 Contact Form

When deployed to Netlify:

- Submissions go to your email
- Configure at Netlify dashboard → Site settings → Forms
- Users redirected to `thanks.html` after submit
- Spam protection via honeypot field

## 🐛 Troubleshooting

| Issue                            | Solution                                                                         |
| -------------------------------- | -------------------------------------------------------------------------------- |
| CV won't download locally        | Use `npm run dev` (file:// protocol doesn't allow downloads)                     |
| GitHub projects not showing      | Check: (1) Username in line 941, (2) API rate limits (60 req/hr unauthenticated) |
| Contact form not working locally | This is expected - works only when deployed to Netlify                           |
| Dark mode not saving             | Check localStorage in browser DevTools                                           |
| Images not loading               | Verify image paths start with `./`                                               |

## 🎯 Next Steps

1. **Test locally:**

   ```bash
   npm run dev
   ```

2. **Deploy to Netlify:**
   - Push to GitHub
   - Connect repo to Netlify
   - Deploy!

3. **Verify everything works:**
   - [ ] Hero section displays with gradient
   - [ ] CV links work
   - [ ] GitHub projects load
   - [ ] Contact form submits
   - [ ] Mobile responsive
   - [ ] Dark/light mode toggle works

## 📚 Resources

- [Tailwind CSS Docs](https://tailwindcss.com)
- [Netlify Forms Docs](https://docs.netlify.com/forms/setup/)
- [GitHub API Docs](https://docs.github.com/en/rest)
- [Netlify Deployment Guide](https://docs.netlify.com/get-started/)

## 📄 License

Personal portfolio project. Feel free to customize and deploy.

---

**Status:** ✅ Ready for deployment

**Last Updated:** June 2026
