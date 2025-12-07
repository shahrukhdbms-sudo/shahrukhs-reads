# Shahrukh's Reads

**History-Provoking Ideas for Modern Research**

A Progressive Web App (PWA) for sharing thought-provoking content that bridges historical foundations with modern research perspectives.

---

## Features

- 📱 **Installable as an App** - Users can install it on their phone/desktop like a native app
- 🔍 **Search Functionality** - Find posts by title or content
- 🏷️ **Category Filtering** - Browse by Historical Foundations, Modern Perspectives, Research Intersections, Thought Experiments, or Featured
- 📤 **Share Posts** - Native sharing on mobile, clipboard copy on desktop
- 📶 **Works Offline** - Once loaded, the app works without internet
- 🎨 **Beautiful Design** - Clean, professional, and academic aesthetic

---

## How to Deploy to GitHub Pages (Free Hosting)

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Follow the registration process

### Step 2: Create a New Repository
1. Click the **+** icon in the top right → **New repository**
2. Name it: `shahrukhs-reads` (or any name you prefer)
3. Make sure **Public** is selected
4. Check **"Add a README file"**
5. Click **Create repository**

### Step 3: Upload the App Files
1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop ALL files from this folder:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. Click **Commit changes**

### Step 4: Enable GitHub Pages
1. Go to your repository **Settings** (gear icon)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**

### Step 5: Access Your App
- Wait 1-2 minutes for deployment
- Your app will be live at: `https://YOUR-USERNAME.github.io/shahrukhs-reads`
- Share this URL with anyone!

---

## How to Add/Edit Content

All your posts are stored in the `index.html` file. To add new posts:

1. Go to your GitHub repository
2. Click on `index.html`
3. Click the **pencil icon** (Edit this file)
4. Find the `const posts = [` section (around line 470)
5. Add a new post following this format:

```javascript
{
    id: 7,  // Use the next number
    title: "Your Post Title",
    category: "modern",  // Options: historical, modern, intersection, thought, featured
    categoryLabel: "Modern Perspectives",  // Display name for the category
    excerpt: "A brief teaser that appears on the card...",
    content: `<p>Your full article content goes here.</p>
    <p>You can have multiple paragraphs.</p>
    <p>Use HTML tags like <strong>bold</strong> or <em>italic</em>.</p>`,
    date: "December 7, 2025",
    readTime: "4 min read"
},
```

6. Click **Commit changes**
7. Your new post will appear on the site within minutes!

### Category Options:
| Category Value | Display Label | Color |
|---------------|---------------|-------|
| `historical` | Historical Foundations | Purple |
| `modern` | Modern Perspectives | Teal |
| `intersection` | Research Intersections | Orange |
| `thought` | Thought Experiments | Pink |
| `featured` | Featured Reads | Gold |

---

## How Users Install the App

### On Android:
1. Open the app URL in Chrome
2. Tap the **"Install"** banner that appears, OR
3. Tap the menu (⋮) → **"Install app"** or **"Add to Home screen"**

### On iPhone/iPad:
1. Open the app URL in Safari
2. Tap the **Share** button (square with arrow)
3. Scroll down and tap **"Add to Home Screen"**
4. Tap **Add**

### On Desktop (Chrome/Edge):
1. Open the app URL
2. Click the **install icon** in the address bar (or the banner)
3. Click **Install**

---

## Customization

### Change Colors
Find the `:root` CSS section at the top of `index.html` and modify:
- `--accent`: The gold accent color
- `--text-primary`: Main text color
- `--bg-primary`: Background color

### Change App Name
1. Update the `<title>` tag in `index.html`
2. Update `name` and `short_name` in `manifest.json`
3. Update the logo text in the header

---

## Support

If you need help, feel free to reach out or open an issue on GitHub.

Made with ♥ for curious minds.
