# FLEX Project Page Restructuring

## 📁 File Structure

The project has been restructured into a modular architecture:

```
flex-gensi-thuair.github.io/
├── index.html              # Main HTML (to be created with new structure)
├── index_original.html     # Original monolithic version
├── index_bak.html          # Backup copy
├── plan.md                 # Detailed restructuring plan
├── css/
│   ├── main.css           # Core styles & design system
│   ├── hero.css           # Hero section specific styles  
│   ├── series.css         # Research series section styles
│   └── animations.css     # All animations & transitions
├── js/
│   ├── main.js            # Core interactions & utilities
│   └── series-manager.js  # Series works management
├── data/
│   └── series-works.json  # Series works database
└── asset/
    └── [images & logos]
```

## 🎯 Key Improvements

### 1. **Modular CSS Architecture**
- Separated concerns: base styles, components, animations
- CSS custom properties for consistent theming
- Easier maintenance and updates
- Better performance with code splitting

### 2. **Enhanced Hero Section**
- Full-viewport animated hero
- Rotating taglines showcasing key concepts
- Floating stat cards with animations
- Scroll indicator for better UX

### 3. **Research Series Section** ⭐
- **New dedicated section** for FLEX research series
- Dynamic content loading from JSON
- Filterable by domain (Math, Chemistry, Biology, etc.)
- Status badges (Published, Preprint, In Progress, Planned)
- Card-based layout for easy expansion
- Core work highlighted prominently

### 4. **Improved Interactivity**
- Smooth scroll with progress indicator
- Animated section reveals on scroll
- Tab functionality for case studies
- Lazy loading for images
- Better mobile menu (responsive)

### 5. **Accessibility & Performance**
- Skip-to-content link
- Proper ARIA labels
- Keyboard navigation support
- Reduced motion support
- Semantic HTML5 structure
- Optimized loading strategy

##  🚀 Quick Start

### Current Status
The restructuring is **in progress**. Currently available:

✅ CSS modules created (main, hero, series, animations)
✅ JavaScript modules created (main, series-manager)
✅ JSON data structure for series works
✅ Detailed plan document (plan.md)
⏳ New index.html integration (next step)

### To Complete the Migration

1. **Review the plan.md** to understand the full vision
2. **Create the new index.html** using the modular approach
3. **Test all features** across devices and browsers
4. **Gradually add series works** to data/series-works.json

## 📝 Adding New Series Works

Edit `data/series-works.json`:

```json
{
  "id": "unique-work-id",
  "title": "Work Title",
  "status": "published|preprint|in_progress|planned",
  "domain": "mathematics|chemistry|biology|methodology|applications|theory",
  "icon": "🔢",
  "description": "Brief description (1-2 sentences)",
  "preview_image": "path/to/image.png",
  "date": "2025 Q2",
  "metrics": {
    "key_improvement": "Improvement description"
  },
  "links": {
    "paper": "URL or null",
    "code": "URL or null"
  },
  "is_core": false
}
```

The page will automatically update to show the new work!

## 🎨 Design System

### Colors
- **Core**: Blue gradient (#2563eb → #3b82f6)
- **Math**: Blue (#3b82f6)
- **Chemistry**: Green (#10b981)
- **Biology**: Purple (#8b5cf6)
- **Methodology**: Amber (#f59e0b)
- **Applications**: Cyan (#06b6d4)
- **Theory**: Indigo (#6366f1)

### Typography
- **Headings**: System fonts, -apple-system, Segoe UI, etc.
- **Body**: 1.1rem, line-height 1.8
- **Code**: Courier New, monospace

### Spacing
- Uses 8px grid system
- Responsive scaling with clamp()

## 🔧 Development

### Local Testing
```bash
# Start a local server
python3 -m http.server 8080

# Open http://localhost:8080
```

### File Watching (Optional)
For live reload during development, use tools like:
- `live-server` (npm)
- VS Code Live Server extension

## 📚 Documentation

- **plan.md**: Comprehensive restructuring plan with rationale
- **CSS files**: Inline comments explaining each section
- **JS files**: JSDoc-style comments for functions

## 🤝 Contributing

When adding new features:

1. Follow the existing file structure
2. Use CSS custom properties for colors
3. Ensure mobile responsiveness
4. Test accessibility (keyboard navigation, screen readers)
5. Add comments for complex logic

## 🔄 Migration Path

### Phase 1: Foundation ✅ COMPLETE
- [x] Create modular file structure
- [x] Extract CSS to external files
- [x] Create JavaScript modules
- [x] Set up data structure

### Phase 2: Integration (NEXT)
- [ ] Create new index.html with modular imports
- [ ] Test hero section animations
- [ ] Verify series section functionality
- [ ] Cross-browser testing

### Phase 3: Content Migration
- [ ] Port remaining original content
- [ ] Add detailed results sections
- [ ] Include case studies
- [ ] Add discussion section

### Phase 4: Polish & Launch
- [ ] Performance optimization
- [ ] Final accessibility audit
- [ ] SEO optimization
- [ ] Deploy to production

## 📞 Questions?

Refer to:
- `plan.md` for detailed rationale
- Original content in `index_original.html`
- CSS comments for styling questions
- JS comments for functionality questions

---

**Last Updated**: 2025-11-09
**Status**: In Progress - Phase 1 Complete
