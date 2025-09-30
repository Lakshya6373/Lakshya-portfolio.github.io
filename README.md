# DevOps Portfolio Website

A dynamic, modern portfolio website with cloud and DevOps theme, built with HTML, CSS, and JavaScript.

## 🚀 Features

- **Responsive Design** - Works perfectly on all devices
- **Dynamic Animations** - Typing effect, glitch effect, smooth scrolling
- **Cloud Theme** - Animated cloud background with DevOps aesthetics
- **Project Filtering** - Filter projects by category
- **Interactive Skills Section** - Animated progress bars
- **Contact Form** - Ready-to-integrate contact functionality
- **Smooth Animations** - Intersection Observer API for scroll animations
- **Mobile Menu** - Hamburger menu for mobile devices

## 📦 How to Deploy on GitHub Pages (FREE)

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in (or create an account)
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Name your repository: `username.github.io` (replace `username` with your GitHub username)
   - For example: `johnsmith.github.io`
   - This special naming will make your site available at `https://username.github.io`
5. Make sure it's set to **Public**
6. Click **"Create repository"**

### Step 2: Push Your Code to GitHub

Open your terminal/PowerShell in the portfolio folder and run:

```powershell
# Initialize git repository
git init

# Add all files
git add .

# Commit your changes
git commit -m "Initial portfolio commit"

# Add your GitHub repository as remote (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"main"** branch
5. Click **"Save"**
6. Wait 1-2 minutes for deployment

### Step 4: Access Your Website

Your website will be live at: `https://YOUR-USERNAME.github.io`

## 🎨 Customization Guide

### Update Personal Information

1. **Open `index.html`** and update:
   - Your name and title in the hero section
   - About me text
   - Projects information
   - Contact details (email, phone, location)
   - Social media links (GitHub, LinkedIn, Twitter, etc.)

2. **Open `js/script.js`** and customize:
   - Typing animation texts (lines 2-8)
   - Any other dynamic content

3. **Open `css/style.css`** to change:
   - Colors (modify CSS variables at the top)
   - Fonts
   - Spacing and layouts

### Add Your Projects

In `index.html`, find the projects section and modify the project cards:

```html
<div class="project-card" data-category="cloud devops">
    <div class="project-icon">
        <i class="fas fa-server"></i>
    </div>
    <h3>Your Project Name</h3>
    <p>Your project description</p>
    <div class="project-tags">
        <span>Technology 1</span>
        <span>Technology 2</span>
    </div>
    <a href="your-project-link" class="project-link">View Details <i class="fas fa-arrow-right"></i></a>
</div>
```

### Update Skills

Modify the skills section to reflect your actual skill levels. Change the `data-progress` values:

```html
<div class="skill-progress" data-progress="90"></div>
```

### Configure Contact Form

The contact form currently shows an alert. To make it functional:

1. **Option 1: Use FormSpree**
   - Go to [formspree.io](https://formspree.io)
   - Create a free account
   - Get your form endpoint
   - Update the form action in `index.html`

2. **Option 2: Use Netlify Forms** (if deploying on Netlify)
   - Add `netlify` attribute to the form
   - Forms will be automatically handled

3. **Option 3: Custom Backend**
   - Create your own API endpoint
   - Update the fetch code in `js/script.js` (line 215)

## 🛠️ Technologies Used

- HTML5
- CSS3 (Grid, Flexbox, Animations)
- JavaScript (ES6+)
- Font Awesome Icons
- Intersection Observer API

## 📱 Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers

## 🎯 SEO Optimization (Optional)

Add to your `index.html` head section:

```html
<meta name="description" content="Your portfolio description">
<meta name="keywords" content="DevOps, Cloud Engineer, AWS, Azure, Docker, Kubernetes">
<meta name="author" content="Your Name">
<meta property="og:title" content="Your Name - DevOps Portfolio">
<meta property="og:description" content="Your portfolio description">
<meta property="og:image" content="https://yourdomain.com/preview-image.jpg">
```

## 📄 Custom Domain (Optional)

To use your own domain name:

1. Buy a domain from any registrar (Namecheap, GoDaddy, etc.)
2. Create a file named `CNAME` in your repository
3. Add your domain name to the file (e.g., `www.yourdomain.com`)
4. Configure your domain's DNS settings:
   - Add A records pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add a CNAME record pointing to `YOUR-USERNAME.github.io`

## 🔄 Updates and Maintenance

To update your website after making changes:

```powershell
git add .
git commit -m "Update portfolio"
git push
```

GitHub Pages will automatically rebuild and deploy your site!

## 📞 Support

If you encounter any issues:
- Check GitHub Pages documentation: https://pages.github.com
- Review GitHub repository settings
- Ensure all files are properly committed and pushed

## 📝 License

Free to use for personal and commercial projects.

## 🌟 Tips

1. **Optimize Images**: Compress images before uploading
2. **Add Analytics**: Use Google Analytics to track visitors
3. **Regular Updates**: Keep your portfolio updated with new projects
4. **Mobile First**: Always test on mobile devices
5. **Performance**: Use tools like Lighthouse to optimize performance

---

**Happy Coding! 🚀**

Built with ❤️ and deployed on GitHub Pages
