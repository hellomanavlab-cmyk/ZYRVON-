# ZYRVON Website - Quick Reference Card

**Print this or keep it open while developing**

---

## 🚀 Start Here

```bash
cd zyrvon-website
npm install
npm run dev
```

Browser opens: `http://localhost:5173`

---

## 🎨 Customize These First

### 1. Change Brand Color
**File:** `src/index.css` (Line 8)
```css
--color-blue: #00d4ff;  /* ← Change this hex color */
```
Entire site updates automatically.

### 2. Update Company Name
**File:** `src/components/Navbar.jsx` (Line 40)
```jsx
<span className="logo-text">YOUR_COMPANY_NAME</span>
```

### 3. Replace Email Address
**Find & Replace:** `hello@zyrvon.com` → `your-email@company.com`

### 4. Update Page Content
Edit any file in `src/pages/`:
```
src/pages/Home.jsx       ← Home page
src/pages/About.jsx      ← About page
src/pages/Solutions.jsx  ← Solutions
src/pages/Projects.jsx   ← Case studies
src/pages/Contact.jsx    ← Contact form
```

---

## 📁 Project Structure (Simplified)

```
src/
├── pages/              ← Edit page content
├── components/         ← Reusable components
│   └── home/          ← Home page visuals
├── index.css          ← Colors, spacing, fonts
└── utils/             ← Animation presets
```

---

## 🎬 Common Tasks

### Add a New Page
1. Create `src/pages/NewPage.jsx`
2. Create `src/pages/NewPage.css`
3. Import in `src/App.jsx`
4. Add route in `<Routes>`
5. Add link in `src/components/Navbar.jsx`

### Add a New Component
1. Create `src/components/NewComponent.jsx`
2. Create `src/components/NewComponent.css`
3. Import where needed

### Change Page Background Color
**File:** `src/pages/YourPage.css`
```css
.your-page {
  background: var(--color-charcoal);  /* or other color */
}
```

### Add an Icon
```jsx
import { IconName } from 'lucide-react'

<IconName size={24} />
```

Browse icons: https://lucide.dev

---

## 🎨 Color Options (Pre-defined)

```css
--color-blue           #00d4ff   (Primary)
--color-blue-dark      #0099cc   (Darker shade)
--color-blue-light     #33e5ff   (Lighter shade)
--color-black          #0a0e1a   (Background)
--color-charcoal       #1a1f2e   (Section bg)
--color-dark           #2a2f3e   (Hover state)
--color-text           #e4e4e7   (Main text)
--color-text-muted     #a1a1a6   (Secondary text)
--color-border         rgba(0, 212, 255, 0.15)
```

---

## 📏 Spacing Options

Use these in CSS:
```css
--spacing-xs   0.5rem
--spacing-sm   1rem
--spacing-md   1.5rem
--spacing-lg   2rem
--spacing-xl   3rem
--spacing-2xl  4rem
--spacing-3xl  6rem
```

Example:
```css
padding: var(--spacing-lg);  /* padding: 2rem; */
gap: var(--spacing-md);      /* gap: 1.5rem; */
```

---

## 🔤 Typography Options

```css
--font-size-xs   0.75rem
--font-size-sm   0.875rem
--font-size-base 1rem
--font-size-lg   1.125rem
--font-size-xl   1.25rem
--font-size-2xl  1.5rem
--font-size-3xl  2rem
--font-size-4xl  2.5rem
--font-size-5xl  3.5rem
```

---

## ⚡ Build & Deploy

### Development
```bash
npm run dev          # Start dev server with hot reload
```

### Production
```bash
npm run build        # Create optimized build
npm run preview      # Preview production build locally
```

### Deploy to Vercel
```bash
npm install -g vercel
vercel
```

### Deploy to Netlify
```bash
npm run build
# Drag dist/ folder to Netlify website
```

---

## 🔧 Useful Commands

```bash
npm install          # Install dependencies
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm update           # Update dependencies
npm list             # List installed packages
```

---

## 🐛 Troubleshooting

### Page Won't Load
1. Check browser console (F12)
2. Look for red error messages
3. Verify import paths are correct
4. Restart dev server (Ctrl+C, then `npm run dev`)

### Styles Not Showing
1. Verify CSS file is imported in component
2. Check CSS variable names are spelled correctly
3. Clear browser cache (Ctrl+Shift+Delete)
4. Restart dev server

### Animation Slow/Choppy
1. Check browser DevTools Performance tab
2. Reduce animation complexity
3. Use `will-change` CSS for optimization
4. Test in Chrome (better animation support)

### Mobile Menu Not Working
1. Check `src/components/Navbar.jsx`
2. Verify `useState` and `setIsMobileMenuOpen` are set up
3. Test at actual mobile size (<768px)

---

## 📚 File Locations

| What | Where |
|------|-------|
| Page Content | `src/pages/PageName.jsx` |
| Page Styles | `src/pages/PageName.css` |
| Component Code | `src/components/ComponentName.jsx` |
| Component Styles | `src/components/ComponentName.css` |
| Global Styles | `src/index.css` |
| Animations | `src/utils/animations.js` |
| Routing | `src/App.jsx` |
| Navigation | `src/components/Navbar.jsx` |
| Footer | `src/components/Footer.jsx` |

---

## 🎯 7 Pages Included

1. **Home** - `/` - Hero, services, projects
2. **About** - `/about` - Philosophy, principles
3. **Solutions** - `/solutions` - 10 automation solutions
4. **How We Build** - `/how-we-build` - Process, approach
5. **Projects** - `/projects` - Case studies
6. **Insights** - `/insights` - Articles, newsletter
7. **Contact** - `/contact` - Form, info

---

## 📞 When You Need Help

**Quick answers:** Check `QUICK_START.md`
**Setup issues:** Check `README.md`
**Troubleshooting:** Check `SETUP_VERIFICATION.md`
**File reference:** Check `FILE_STRUCTURE.md`
**Project overview:** Check `PROJECT_SUMMARY.md`

---

## ⏱️ Typical Timeline

- **Setup**: 5 minutes (`npm install && npm run dev`)
- **Basic customization**: 30 minutes
- **Detailed customization**: 1-2 hours
- **Deploy**: 5 minutes
- **Live**: Immediate

---

## 🎓 Learning Resources

- React: https://react.dev
- Vite: https://vitejs.dev
- Framer Motion: https://www.framer.com/motion
- React Router: https://reactrouter.com
- Lucide Icons: https://lucide.dev

---

## ✅ Before Going Live

- [ ] Company name updated
- [ ] Email address replaced
- [ ] Colors customized
- [ ] Page content updated
- [ ] Mobile design tested
- [ ] All links working
- [ ] No console errors
- [ ] Built: `npm run build`
- [ ] Deployed to host
- [ ] Live site verified

---

## 💡 Pro Tips

1. **Change all colors at once:** Edit `src/index.css` CSS variables
2. **Add pages quickly:** Copy existing page structure
3. **Reuse components:** Use Section, Button, Card patterns
4. **Test animations:** Use browser DevTools Performance tab
5. **Deploy quickly:** Vercel auto-deploys from Git

---

## 🚀 You're Ready!

**Next step:** Read `QUICK_START.md` or just run:

```bash
cd zyrvon-website
npm install
npm run dev
```

---

**Print or bookmark this page for quick reference!**

**Happy coding!** 🎉
