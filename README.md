# Álvaro Torres - Personal Website

A minimal, clean personal portfolio website built with pure HTML and CSS.

## Tech Stack

- **HTML5** - Structure
- **CSS3** - Styling
- No JavaScript, no frameworks, no build process

## Local Development

Simply open `index.html` in your browser. No server needed.

---

## Deployment Options

### Option 1: GitHub Pages (FREE) - Recommended

1. **Create a GitHub repository**
   ```
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. **Push to GitHub**
   - Create a new repository on GitHub named `alvarotorres.com` (or any name)
   - Push your code:
   ```
   git remote add origin https://github.com/YOUR_USERNAME/alvarotorres.com.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `root`
   - Click Save
   - Your site will be live at `https://YOUR_USERNAME.github.io/alvarotorres.com`

### Option 2: Vercel (FREE)

1. Push your code to GitHub (same as above)
2. Go to [vercel.com](https://vercel.com)
3. Sign in with GitHub
4. Click "Import Project" → Select your repository
5. Click "Deploy"
6. Your site will be live at `https://your-project.vercel.app`

### Option 3: Netlify (FREE)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Done! Your site is live

---

## Custom Domain: alvarotorres.com

### Step 1: Buy the Domain

**Cheapest options (~$10-15/year):**

1. **Cloudflare Registrar** - At-cost pricing, no markup
   - https://www.cloudflare.com/products/registrar/
   
2. **Porkbun** - Often cheapest, ~$9/year for .com
   - https://porkbun.com
   
3. **Namecheap** - ~$10-13/year for .com
   - https://namecheap.com

4. **Google Domains** (now Squarespace) - ~$12/year
   - https://domains.squarespace.com

### Step 2: Connect Domain to Your Host

#### For GitHub Pages:

1. **Add CNAME file to your repo**
   - Create a file named `CNAME` (no extension) in your repo root
   - Add just one line: `alvarotorres.com`

2. **Configure DNS at your registrar**
   - Add these DNS records:
   
   | Type  | Name | Value                      |
   |-------|------|----------------------------|
   | A     | @    | 185.199.108.153           |
   | A     | @    | 185.199.109.153           |
   | A     | @    | 185.199.110.153           |
   | A     | @    | 185.199.111.153           |
   | CNAME | www  | YOUR_USERNAME.github.io   |

3. **Enable in GitHub**
   - Go to repo Settings → Pages → Custom domain
   - Enter: `alvarotorres.com`
   - Check "Enforce HTTPS"

#### For Vercel:

1. Go to your Vercel project → Settings → Domains
2. Add `alvarotorres.com`
3. Vercel will show you DNS records to add
4. Add these records at your registrar
5. Wait for DNS propagation (up to 48h, usually minutes)

#### For Netlify:

1. Go to Site settings → Domain management
2. Add custom domain
3. Follow DNS instructions provided

---

## Cost Summary

| Item | Cost |
|------|------|
| Hosting (GitHub Pages/Vercel/Netlify) | FREE |
| Domain (.com) | ~$10-15/year |
| **Total** | **~$10-15/year** |

---

## File Structure

```
alvarotorres.com/
├── index.html      # Main HTML file
├── style.css       # All styles
├── CNAME           # For GitHub Pages custom domain (create when deploying)
└── README.md       # This file
```

---

## Customization

1. **Edit your info** - Open `index.html` and replace:
   - Your name and tagline
   - Your bio/description
   - All project entries (copy the `<li class="project">` template)
   - Social links in footer

2. **Change colors** - Open `style.css` and edit the `:root` variables:
   ```css
   :root {
       --text: #1a1a1a;
       --text-secondary: #666;
       --background: #fafafa;
       --link: #0066cc;
       --link-hover: #004499;
       --border: #e0e0e0;
   }
   ```

3. **Change font** - Edit the `font-family` in the `body` selector

---

## Quick Deploy Checklist

- [ ] Edit `index.html` with your information
- [ ] Test locally by opening `index.html`
- [ ] Create GitHub repository
- [ ] Push code to GitHub
- [ ] Enable GitHub Pages
- [ ] Buy domain from Cloudflare/Porkbun/Namecheap
- [ ] Create `CNAME` file with your domain
- [ ] Configure DNS records
- [ ] Wait for propagation
- [ ] Verify HTTPS is working

Your site should be live at **https://alvarotorres.com** 🎉
