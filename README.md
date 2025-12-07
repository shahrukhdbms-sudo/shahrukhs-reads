# Shahrukh's Reads - Magazine Edition

**History-Provoking Ideas for Modern Research**

A modern, magazine-style Progressive Web App featuring a dark theme, notification system for unread posts, and elegant typography.

---

## ✨ New Features

- 🌙 **Dark Magazine Theme** - Elegant, eye-friendly dark mode design
- 🔔 **Notification Panel** - Shows unread posts so readers never miss new content
- ⭐ **Featured Article** - Highlight your best content prominently
- 📖 **Reading Tracking** - Automatically tracks which posts users have read
- 🎨 **Modern Typography** - Playfair Display + Source Sans 3 font pairing
- 📱 **Fully Responsive** - Perfect on mobile, tablet, and desktop
- 📤 **Share Articles** - Native sharing on mobile devices
- 📶 **Works Offline** - Full offline capability

---

## How to Update Your GitHub Repository

Since you already have a repository, follow these steps to update it:

### Option A: Replace All Files (Easiest)

1. Go to your repository: `github.com/shahrukhdbms-sudo/shahrukhs-reads`
2. For each file (`index.html`, `manifest.json`, `sw.js`):
   - Click on the file
   - Click the **pencil icon** (✏️) to edit
   - Select all and delete the content
   - Paste the new content from the downloaded files
   - Click **Commit changes**
3. For icon files (`icon-192.png`, `icon-512.png`):
   - Delete the old ones (click file → three dots → Delete file)
   - Upload the new ones (Add file → Upload files)

### Option B: Delete and Re-upload Everything

1. Go to **Settings** → scroll to bottom → **Delete this repository**
2. Create a new repository with the same name
3. Upload all new files

---

## 📝 How to Add New Posts

Find the `const posts = [` section in `index.html` and add:

```javascript
{
    id: 7,  // Next number
    title: "Your Article Title",
    category: "modern",  // Options: historical, modern, intersection, thought, featured
    categoryLabel: "Modern Perspectives",
    excerpt: "A compelling teaser for your article...",
    content: `<p>Your full article content here.</p>
    <p>Add more paragraphs as needed.</p>`,
    date: "December 7, 2025",
    readTime: "5 min read",
    featured: false  // Set to true for featured article
},
```

### Category Options

| Value | Label | Color |
|-------|-------|-------|
| `historical` | Historical Foundations | Purple |
| `modern` | Modern Perspectives | Teal |
| `intersection` | Research Intersections | Gold |
| `thought` | Thought Experiments | Purple/Pink |
| `featured` | Featured | Gold |

---

## 🔔 How the Notification System Works

- When you add new posts, they automatically appear as "unread" for all readers
- A red badge shows the count of unread posts
- Clicking the bell icon opens the notification panel
- Posts are marked as "read" when opened
- "Mark all as read" clears all notifications
- Read status is stored in the user's browser (localStorage)

---

## 🎨 Customization

### Change the Accent Color
Find `:root` at the top of `index.html` and modify:
```css
--accent-red: #e63946;  /* Main accent */
--accent-gold: #d4a373; /* Secondary accent */
```

### Change App Name
1. Update the `<title>` tag
2. Update `.nav-brand` and `.footer-brand` text
3. Update `name` in `manifest.json`

### Make an Article Featured
Set `featured: true` on one article. Only one article should be featured at a time.

---

## 📱 Installing the App

### Android
1. Open in Chrome
2. Tap "Install" banner or Menu → "Add to Home screen"

### iPhone/iPad
1. Open in Safari
2. Tap Share → "Add to Home Screen"

### Desktop
1. Open in Chrome/Edge
2. Click install icon in address bar

---

## Support

For help or feature requests, feel free to reach out!

Made with ♥ for curious minds.
