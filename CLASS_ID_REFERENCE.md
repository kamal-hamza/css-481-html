# Classes and IDs Reference Guide

## Header Section

**IDs:**
- `#main-header` - Main site header

**Classes:**
- `.site-header` - Header styling
- `.site-title` - Main h1 title
- `.navigation` - Navigation container
- `.nav-list` - Navigation ul
- `.nav-item` - Navigation li items
- `.nav-link` - Navigation links
- `.nav-link.active` - Active page indicator

---

## Main Content Section

**IDs:**
- `#main-content` - Main content wrapper

**Classes:**
- `.content-wrapper` - Main content container
- `.main-article` - Main article container
- `.article-title` - Article h2 titles
- `.content-section` - Content sections
- `.section-title` - Section h3 titles

---

## Special Sections

**IDs:**
- `#introduction` - Introduction section (index.html)
- `#interests` - Interests section (index.html)
- `#fun-facts` - Fun facts section (index.html)
- `#goals` - Goals section (index.html)
- `#quote` - Quote section (index.html)
- `#contact` - Contact section (index.html)
- `#sidebar` - Sidebar aside

**Classes:**
- `.highlight-section` - Highlighted content sections
- `.quote-section` - Quote sections
- `.contact-section` - Contact sections
- `.stats-section` - Statistics sections

---

## Games Page Sections

**IDs:**
- `#gaming-intro` - Gaming introduction
- `#gaming-stats` - Gaming statistics table
- `#game-aoe2` - Age of Empires section
- `#game-nfs` - Need for Speed section
- `#game-pvz` - Plants vs Zombies section

**Classes:**
- `.game-section` - Game content sections
- `.game-title` - Game h3 titles
- `.game-subtitle` - Game h4 subtitles
- `.game-quote` - Game blockquotes
- `.game-info` - Game information lists
- `.game-details` - Game detail lists
- `.game-highlight` - Highlighted game content
- `.game-figure` - Game figures
- `.game-version` - Game version headings
- `.game-modes-list` - Game modes lists
- `.character-list` - Character lists
- `.character-team` - Character team headings

---

## Books Page Sections

**IDs:**
- `#books-intro` - Books introduction
- `#reading-stats` - Reading statistics table
- `#book-harry-potter` - Harry Potter section
- `#book-geronimo` - Geronimo Stilton section
- `#book-wimpy-kid` - Diary of a Wimpy Kid section

**Classes:**
- `.book-section` - Book content sections
- `.book-title` - Book h3 titles
- `.book-subtitle` - Book h4 subtitles
- `.book-quote` - Book blockquotes
- `.book-info` - Book information lists

---

## Common Content Classes

**Text Content:**
- `.definition-list` - Definition lists
- `.facts-list` - Facts ordered lists
- `.goals-list` - Goals unordered lists
- `.reasons-list` - Reasons ordered lists
- `.favorites-list` - Favorites unordered lists
- `.features-list` - Features lists
- `.community-list` - Community lists

**Tables:**
- `.data-table` - Data tables
- `.table-caption` - Table captions
- `.cars-table` - Cars table (NFS)
- `.modes-table` - Game modes table (PvZ)

**Special Elements:**
- `.featured-quote` - Featured blockquotes
- `.fact-quote` - Fact blockquotes
- `.subsection-title` - h5 subsection titles
- `.fact-title` - Fact h6 titles

**Ratings:**
- `.rating` - Rating paragraphs
- `.rating-meter` - Rating meter elements

---

## Sidebar & Aside Elements

**IDs:**
- `#sidebar` - Main sidebar

**Classes:**
- `.sidebar` - Sidebar container
- `.sidebar-title` - Sidebar h4 title
- `.sidebar-links` - Sidebar links list
- `.sidebar-item` - Sidebar list items
- `.sidebar-link` - Sidebar anchor links
- `.fun-fact` - Fun fact aside boxes
- `.stat-value` - Statistical data values

---

## Footer Section

**IDs:**
- `#main-footer` - Main site footer

**Classes:**
- `.site-footer` - Footer styling
- `.copyright` - Copyright paragraph
- `.last-updated` - Last updated paragraph
- `.footer-links` - Footer links paragraph
- `.footer-link` - Footer anchor links
- `.footer-nav` - Footer navigation

---

## Selector Specificity Examples

**Highest Specificity (with IDs):**
```css
main#main-content article.main-article section.content-section
→ (1, 3, 2) = 1 ID, 3 classes, 2 elements
```

**High Specificity (classes only):**
```css
header.site-header nav.navigation ul.nav-list li.nav-item a.nav-link
→ (0, 3, 5) = 0 IDs, 3 classes, 5 elements
```

**Medium Specificity:**
```css
footer.site-footer p.footer-links a.footer-link
→ (0, 3, 3) = 0 IDs, 3 classes, 3 elements
```

---

## Usage Examples

### Navigation Link:
```html
<nav class="navigation">
  <ul class="nav-list">
    <li class="nav-item">
      <a href="index.html" class="nav-link active">Home</a>
    </li>
  </ul>
</nav>
```

### Content Section:
```html
<section id="gaming-intro" class="content-section">
  <h3 class="section-title">Why Gaming Matters</h3>
  <p>Content here...</p>
</section>
```

### Table:
```html
<table class="data-table">
  <caption class="table-caption">Statistics</caption>
  <thead>...</thead>
  <tbody>...</tbody>
</table>
```

### Sidebar:
```html
<aside id="sidebar" class="sidebar">
  <h4 class="sidebar-title">Quick Links</h4>
  <ul class="sidebar-links">
    <li class="sidebar-item">
      <a href="#" class="sidebar-link">Link</a>
    </li>
  </ul>
</aside>
```

---

## Total Count

- **IDs:** 15+
- **Classes:** 50+
- **Animations:** 7
- **Transitions:** Applied to 30+ selectors
- **Hover Effects:** Applied to 40+ selectors
- **Cursor Types:** 5 different types

---

## Benefits of This Approach

✅ **No Conflicts:** Highly specific selectors prevent CSS conflicts
✅ **No !important:** Proper specificity eliminates need for overrides
✅ **Maintainable:** Clear naming conventions make updates easy
✅ **Semantic:** Class names describe content purpose
✅ **Reusable:** Common classes (.content-section, .section-title) used throughout
✅ **Scalable:** Easy to add new sections following same pattern

