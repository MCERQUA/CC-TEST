# Contractor Website

A professional website for a local contracting company built with Eleventy (11ty) static site generator. Features a dynamic blog system that automatically generates pages from Markdown files.

## Features

- **Dynamic Blog System**: Automatically generates blog posts from Markdown files in the `/blog` directory
- **Responsive Design**: Mobile-friendly layout that works on all devices
- **Fast Performance**: Static site generation for lightning-fast load times
- **SEO Friendly**: Clean URLs and semantic HTML
- **Easy Content Management**: Add new blog posts by simply creating MD files
- **Netlify Ready**: Pre-configured for automatic deployment on Netlify

## Project Structure

```
contractor-website/
├── blog/                    # Blog posts in Markdown format
├── src/                     # Source files
│   ├── _data/              # Site data (company info, etc.)
│   ├── _includes/          # Layout templates
│   ├── css/                # Stylesheets
│   └── *.njk               # Page templates
├── .eleventy.js            # Eleventy configuration
├── netlify.toml            # Netlify deployment settings
└── package.json            # Project dependencies
```

## Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm start
   ```

3. Open your browser to `http://localhost:8080`

## Adding Blog Posts

To add a new blog post:

1. Create a new `.md` file in the `/blog` directory
2. Use this frontmatter template:
   ```markdown
   ---
   layout: post.njk
   title: "Your Post Title"
   date: 2024-03-01
   author: "Author Name"
   excerpt: "Brief description of the post"
   tags: ["tag1", "tag2"]
   ---
   
   Your post content here...
   ```

3. The blog will automatically update when you save the file (in development) or when Netlify redeploys

## Deployment to Netlify

### Option 1: Deploy with Git

1. Push this project to a GitHub repository
2. Log in to [Netlify](https://app.netlify.com)
3. Click "New site from Git"
4. Choose your repository
5. Deploy settings are pre-configured in `netlify.toml`
6. Click "Deploy site"

### Option 2: Drag & Drop

1. Build the site locally:
   ```bash
   npm run build
   ```
2. Drag the `_site` folder to Netlify's deployment area

## Automatic Deployment

Once connected to Netlify:
- Any push to your main branch triggers a new deployment
- Adding/editing MD files in the `/blog` directory will automatically update the site
- Changes typically go live within 1-2 minutes

## Customization

### Company Information
Edit `src/_data/site.json` to update:
- Company name
- Contact information
- Social media links

### Styling
Modify `src/css/style.css` to change:
- Colors (defined as CSS variables)
- Typography
- Layout spacing

### Pages
Edit the `.njk` files in the `src` directory to modify page content

## Build Output

The built site is generated in the `_site` directory. This is what gets deployed to Netlify.

## Project Overview
- **Project:** ICA Website (Insulation Contractors of Arizona)
- **Framework:** Eleventy (11ty) static site generator
- **Deployment:** Netlify
- **Current Directory:** e:/1-WORKING-NEW/Mike/AZFOAM/ICA-Website

## Critical Layout Rules

### ⚠️ IMPORTANT: Layout References
When creating or editing service pages, ALWAYS use the full layout path:
- ✅ Correct: `layout: layouts/service-page.njk`
- ❌ Incorrect: `layout: service-page.njk`

**Why:** Eleventy requires the full path when layouts are in subdirectories within `_includes/`

**Files Affected:** All files in `src/services/` subdirectories

### Layout File Locations
- Service pages: `src/_includes/layouts/service-page.njk`
- Regular pages: `src/_includes/layouts/page.njk`
- Service categories: `src/_includes/layouts/service-category.njk`

## File Structure Guidelines

### Service Files Organization
```
src/services/
├── residential/
├── commercial/
├── industrial/
└── agricultural/
```

### Layout Files Organization
```
src/_includes/
├── layouts/
│   ├── page.njk
│   ├── service-page.njk
│   └── service-category.njk
├── components/
└── sections/
```

## Common Issues Prevention

### 1. Layout Reference Errors
- **Issue:** Netlify deployment fails with layout not found errors
- **Prevention:** Always use full layout paths
- **Quick Fix:** Run `node fix-layouts.js`

### 2. Missing Template Files
- **Issue:** Service files include sections that don't exist
- **Prevention:** Verify all included sections exist before deployment
- **Quick Fix:** Create missing section files or update includes

### 3. New Service Page Creation
When creating new service pages:
1. Use correct layout reference: `layout: layouts/service-page.njk`
2. Follow existing frontmatter structure
3. Include required fields: title, subtitle, meta_description, benefits, process
4. Verify all included sections exist in `src/_includes/sections/`

## Deployment Guidelines

### Before Pushing Changes
1. Test locally with `npm run dev`
2. Verify layout references are correct
3. Check for any console errors
4. Ensure all required frontmatter fields are present

### Emergency Fixes
- Layout issues: Run `node fix-layouts.js`
- Check `docs/common-issues.md` for known solutions

## Development Notes
- Last layout fix: 2025-05-30 (Fixed 4 files)
- Fixed files: crawl-space.njk, wall.njk, removal.njk, office.njk
- Script location: `fix-layouts.js` (root directory)

## Contact Information
- Project: ICA Website
- Phone: 623-241-1939
- Focus: Arizona insulation services
