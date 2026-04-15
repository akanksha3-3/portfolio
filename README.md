# Personal Portfolio Website - Akanksha Waghamode

## 📋 Project Overview

### Project Description
A fully responsive personal portfolio website designed to showcase my skills, projects, and professional experience in Data Science and Bioinformatics. This project demonstrates proficiency in modern web development technologies and follows industry-standard best practices for responsive design, accessibility, and user experience.

### Goals and Objectives
- **Primary Goal**: Create a professional online presence to showcase my work and expertise in Data Science and Bioinformatics
- **Learning Objectives**: 
  - Master HTML5 semantic elements and document structure
  - Implement CSS3 modern layout techniques (Flexbox and Grid)
  - Build responsive designs using mobile-first approach
  - Ensure web accessibility compliance (WCAG 2.1 guidelines)
  - Practice form validation and user interaction
- **Career Goal**: Provide a central hub for potential employers, collaborators, and the professional community to learn about my work

---

## 🚀 Features

### Core Features
1. **Responsive Navigation**
   - Sticky header with smooth scrolling
   - Mobile hamburger menu for small screens
   - Active section highlighting on scroll

2. **Home Section**
   - Eye-catching introduction with gradient background
   - Call-to-action buttons
   - Social media integration

3. **About Section**
   - Professional biography
   - Statistics cards (Projects, Internships, Certifications)
   - Two-column responsive layout

4. **Skills Section**
   - Categorized skill display (Programming, Data Science, Bioinformatics, Visualization)
   - Interactive hover effects
   - Tag-based organization

5. **Projects Showcase**
   - Grid layout with project cards
   - Project images with hover effects
   - Technology tags
   - Direct links to GitHub repositories

6. **Experience Timeline**
   - Chronological display of work experience and education
   - Visual timeline with markers
   - Hover animations

7. **Contact Form**
   - Integrated with FormSpree for email handling
   - Client-side validation
   - Responsive layout
   - Anti-spam protection

8. **Accessibility Features**
   - Semantic HTML5 elements
   - ARIA labels and roles
   - Keyboard navigation support
   - High contrast color scheme
   - Alt text for images

---

## 🛠️ Technologies Used

### Frontend Technologies
- **HTML5**: Semantic markup, accessibility features
- **CSS3**: Modern styling with advanced features
  - CSS Grid for layout
  - Flexbox for alignment
  - CSS Variables for theming
  - Media queries for responsiveness
  - Animations and transitions
- **JavaScript (ES6+)**: Interactive features
  - DOM manipulation
  - Event handling
  - Form validation
  - Scroll animations

### External Services
- **FormSpree**: Contact form backend (https://formspree.io)
- **Font Awesome**: Icon library (v6.5.0)
- **GitHub Pages**: Hosting platform

### Development Tools
- **VS Code**: Code editor
- **Git**: Version control
- **Chrome DevTools**: Testing and debugging
- **W3C Validators**: HTML/CSS validation

---

## 📁 Project Structure

```
week1-portfolio/
│
├── index.html                  # Main HTML file (entry point)
│
├── css/
│   ├── variables.css          # CSS custom properties (design tokens)
│   ├── style.css              # Main stylesheet
│   └── responsive.css         # Media queries for responsive design
│
├── js/
│   └── navigation.js          # JavaScript for interactivity
│
├── images/                    # Project images and assets
│   ├── docking.png           # Molecular docking project image
│   ├── house.jpeg            # House price prediction project
│   ├── breast-cancer.jpg     # Cancer classification project
│   ├── data-augmentation.jpeg # Data augmentation project
│   └── news.jpg              # News aggregator project
│
├── README.md                  # Project documentation (this file)
└── .gitignore                # Git ignore file

```

### File Descriptions

#### HTML Files
- **index.html**: Main HTML document containing all sections (Home, About, Skills, Projects, Experience, Contact)

#### CSS Files
- **variables.css**: Contains all CSS custom properties for colors, typography, spacing, shadows, and breakpoints
- **style.css**: Main stylesheet with all component styles, layout rules, and base styles
- **responsive.css**: Media queries for different screen sizes (mobile, tablet, desktop)

#### JavaScript Files
- **navigation.js**: Handles mobile menu toggle, smooth scrolling, form validation, and scroll animations

#### Image Assets
- Visual content (stored in `images/` directory)

---

## 🎨 Design Architecture

### Color Scheme
```css
Primary Color: #667eea (Purple)
Secondary Color: #764ba2 (Deep Purple)
Accent Color: #f093fb (Pink)
Background: #f7fafc (Light Gray)
Text Primary: #2d3748 (Dark Gray)
Text Secondary: #4a5568 (Medium Gray)
```

### Typography
- **Primary Font**: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- **Heading Sizes**: 
  - H1: 3rem (48px)
  - H2: 2.25rem (36px)
  - H3: 1.5rem (24px)
- **Body Text**: 1rem (16px)

### Layout Structure
1. **CSS Grid**: Used for project cards, skills grid, and contact section
2. **Flexbox**: Used for navigation, buttons, and card content alignment
3. **Box Model**: Proper spacing with margin, padding, and border

### Responsive Breakpoints
```css
Mobile: < 480px
Tablet: 481px - 768px
Desktop: 769px - 1024px
Large Desktop: > 1024px
```

---

## 📚 Technical Implementation

### HTML5 Semantic Structure

The website uses semantic HTML5 elements for better accessibility and SEO:

```html
<header>          <!-- Site header with navigation -->
<nav>             <!-- Navigation menu -->
<main>            <!-- Main content wrapper -->
  <section>       <!-- Content sections -->
  <article>       <!-- Project cards -->
<footer>          <!-- Site footer -->
```

**Key Semantic Elements Used**:
- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`
- ARIA labels: `role="banner"`, `role="navigation"`, `aria-label`, `aria-labelledby`
- Proper heading hierarchy (H1 → H2 → H3)

### CSS Architecture

#### 1. **CSS Variables (Custom Properties)**
Centralized design tokens for maintainability:
```css
:root {
  --primary-color: #667eea;
  --spacing-md: 1rem;
  --font-size-xl: 1.25rem;
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}
```

#### 2. **Box Model Implementation**
Every element follows the box model: Content → Padding → Border → Margin
```css
.project-card {
  padding: 32px;        /* Internal spacing */
  margin: 16px;         /* External spacing */
  border: 2px solid;    /* Border */
}
```

#### 3. **CSS Grid Layout**
```css
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 32px;
}
```

#### 4. **Flexbox Layout**
```css
.nav-links {
  display: flex;
  gap: 32px;
  align-items: center;
}
```

#### 5. **CSS Positioning**
- **Sticky**: Header navigation (`position: sticky`)
- **Relative**: Parent containers for absolute children
- **Absolute**: Timeline markers, pseudo-elements
- **Fixed**: Mobile menu overlay

### Responsive Design Implementation

#### Mobile-First Approach
Base styles written for mobile, then enhanced for larger screens:

```css
/* Base (Mobile) */
.container { padding: 0 16px; }

/* Tablet and up */
@media (min-width: 768px) {
  .container { padding: 0 24px; }
}
```

#### Media Queries Structure
```css
/* Large Tablets: max-width 1024px */
@media screen and (max-width: 1024px) { }

/* Tablets: max-width 768px */
@media screen and (max-width: 768px) { }

/* Mobile: max-width 480px */
@media screen and (max-width: 480px) { }
```

### JavaScript Functionality

#### 1. **Mobile Navigation Toggle**
```javascript
burger.addEventListener('click', () => {
  burger.classList.toggle('active');
  navLinks.classList.toggle('active');
});
```

#### 2. **Smooth Scrolling**
```javascript
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();
    // Smooth scroll implementation
  });
});
```

#### 3. **Form Validation**
```javascript
function validateInput(input) {
  // Email regex validation
  // Required field checks
  // Display error messages
}
```

#### 4. **Scroll Animations**
```javascript
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.style.opacity = '1';
    }
  });
});
```

### Accessibility Implementation

#### 1. **Keyboard Navigation**
- All interactive elements accessible via Tab key
- Focus states visible
- Logical tab order

#### 2. **Screen Reader Support**
```html
<nav role="navigation" aria-label="Main navigation">
<button aria-label="Toggle menu" aria-expanded="false">
```

#### 3. **Color Contrast**
- Text-to-background ratio: 4.5:1 (WCAG AA compliant)
- Interactive elements have clear visual feedback

#### 4. **Form Accessibility**
```html
<label for="email">Email *</label>
<input type="email" id="email" required aria-required="true">
```

---

## 💻 Setup Instructions

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A text editor (VS Code recommended)
- Git (optional, for version control)
- Internet connection (for external resources: Font Awesome, FormSpree)

### Installation Steps

#### Step 1: Download/Clone the Project
```bash
# Option 1: Clone from GitHub
git clone https://github.com/akanksha3-3/portfolio.git
cd portfolio

# Option 2: Download ZIP file
# Extract to desired location
```

#### Step 2: Project Structure Setup
Ensure your folder structure matches:
```
portfolio/
├── index.html
├── css/
│   ├── variables.css
│   ├── style.css
│   └── responsive.css
├── js/
│   └── navigation.js
└── images/
    └── (your images)
```

#### Step 3: Add Your Images
1. Place your project images in the `images/` folder
2. Update image paths in `index.html` if necessary:
```html
<img src="images/your-project.jpg" alt="Project description">
```

#### Step 4: Customize Content

**Personal Information (index.html)**:
- Lines 45-48: Update name and title
- Lines 67-81: Update social media links
- Lines 97-111: Update About section text
- Lines 314-330: Update contact information

**Skills (index.html)**:
- Lines 136-177: Customize your skills list

**Projects (index.html)**:
- Lines 184-293: Update project details, images, and GitHub links

**Colors (css/variables.css)**:
```css
/* Change primary color */
--primary-color: #your-color;
```

#### Step 5: Test Locally

**Option A: Direct File Opening**
1. Right-click `index.html`
2. Select "Open with" → Your browser

**Option B: Local Server (Recommended)**

Using Python:
```bash
# Navigate to project folder
cd week1-portfolio

# Start server
python -m http.server 8000

# Open in browser
http://localhost:8000
```

Using VS Code Live Server:
1. Install "Live Server" extension
2. Right-click `index.html`
3. Select "Open with Live Server"

Using Node.js:
```bash
npx http-server
```

---

## 🧪 Testing Evidence

### 1. Responsiveness Testing

#### Desktop View (1920x1080)
✅ **Tested Features**:
- Full navigation menu displays horizontally
- 3-column project grid layout
- 2-column about section
- All sections properly aligned
- Hover effects working

#### Mobile View (375px)
✅ **Tested Features**:
- Hamburger menu functional
- All content single-column
- Buttons full-width
- Text readable without zoom
- Images scale properly

**Testing Methods**:
- Chrome DevTools Device Toolbar
- Responsive Design Mode in Firefox
- Physical device testing (iOS, Android)
- BrowserStack for cross-device testing

### 2. Form Validation Testing

#### Test Cases:

**Test Case 1: Empty Form Submission**
- **Input**: Submit form with all fields empty
- **Expected**: Error messages for all required fields
- **Result**: ✅ Pass - All fields show "Field is required"

**Test Case 2: Invalid Email Format**
- **Input**: Email = "test@invalid"
- **Expected**: "Please enter a valid email address"
- **Result**: ✅ Pass

**Test Case 3: Short Name Input**
- **Input**: Name = "A"
- **Expected**: "Name must be at least 2 characters"
- **Result**: ✅ Pass

**Test Case 4: Short Message**
- **Input**: Message = "Hi"
- **Expected**: "Message must be at least 10 characters"
- **Result**: ✅ Pass

**Test Case 5: Valid Form Submission**
- **Input**: All fields filled correctly
- **Expected**: Success message, form reset, email sent via FormSpree
- **Result**: ✅ Pass - FormSpree confirmation received

### 3. Accessibility Testing

#### WCAG 2.1 Compliance Checklist:

✅ **Level A Requirements**:
- [x] Text alternatives for images
- [x] Keyboard accessible
- [x] Sufficient color contrast (4.5:1 ratio)
- [x] Logical heading hierarchy
- [x] Form labels properly associated

✅ **Level AA Requirements**:
- [x] Enhanced color contrast (7:1 for large text)
- [x] Resize text up to 200% without loss of content
- [x] Multiple ways to navigate (menu, skip links)
- [x] Focus visible on all interactive elements

**Testing Tools Used**:
- WAVE (Web Accessibility Evaluation Tool)
- Keyboard-only navigation test
- Screen reader test

### 4. Code Validation

#### HTML Validation (W3C Validator)
- **URL**: https://validator.w3.org/
- **Result**: 0 errors, 3 warnings

#### CSS Validation (W3C CSS Validator)
- **URL**: https://jigsaw.w3.org/css-validator/
- **Result**:  0 errors
- **Warnings**: 421 (vendor prefixes and CSS variables - expected)

### 5. Performance Testing

#### Load Time Analysis (Desktop):
- **First Contentful Paint**: 0.6s
- **Largest Contentful Paint**: 0.6s
- **Total Blocking Time**: 0 ms
- **Cumulative Layout Shift**: 0
- **Speed Index**: 0.9s

#### Optimization Techniques Applied:
- ✅ Minified CSS (production ready)
- ✅ Optimized images (compressed JPEG/PNG)
- ✅ External resources loaded via CDN
- ✅ CSS loaded in `<head>`, JS at end of `<body>`

### 6. Interactive Elements Testing

#### Buttons and Links:
- ✅ All hover effects working
- ✅ Active states visible
- ✅ Focus outlines present
- ✅ GitHub links open in new tabs
- ✅ Email links open mail client
- ✅ Phone links trigger call on mobile

#### Animations:
- ✅ Hero gradient animation smooth
- ✅ Project cards hover animation
- ✅ Skill tags hover effect
- ✅ Scroll-triggered fade-ins
- ✅ No animation jank (60fps maintained)

---

## 📸 Visual Documentation

### Screenshots

#### 1. Desktop View - Home Section
```
![Portfolio](https://raw.githubusercontent.com/akanksha3-3/portfolio/main/images/home.png)

Features Demonstrated:
- Responsive typography (H1: 48px)
- Gradient background with animation
- Flexbox button layout
- Social media integration
```

#### 2. Desktop View - Skills Section
```
![portfolio](img/skills.png)

Features Demonstrated:
- CSS Grid (4 columns)
- Hover effects on cards
- Tag-based skill organization
- Category headers with icons
```

#### 3. Desktop View - Projects Section
```
![portfolio](img/project.png)

Features Demonstrated:
- CSS Grid responsive layout
- Image hover zoom effect
- Technology tags
- GitHub links
```

#### 4. Mobile View - Full Page
```
![portfolio](img/mobile-view.png)

Features Demonstrated:
- Mobile-first design
- Full-width buttons
- Readable typography
- Optimized spacing
```

#### 5. Mobile View - Menu Open
```
![portfolio](img/mobile-menu.png)

Features Demonstrated:
- Mobile menu animation
- Accessible close button
- Touch-friendly tap targets
```

#### 6. Contact Form - Validation
```
![portfolio](img/contact-form.png)

Features Demonstrated:
- Real-time validation
- Error message styling
- Focus states
- Accessible form labels
```

## 🔧 Algorithms and Data Structures

### 1. Form Validation Algorithm

```javascript
/**
 * Validates user input in contact form
 * Algorithm: Sequential validation with early return
 * Time Complexity: O(1) - constant time per field
 */

function validateForm() {
  // Initialize validation state
  let isValid = true;
  
  // Clear previous errors
  clearErrors(); // O(n) where n = number of fields
  
  // Validation rules (sequential checks)
  
  // 1. Name validation
  if (name.length === 0) {
    showError('nameError', 'Name is required');
    isValid = false;
  } else if (name.length < 2) {
    showError('nameError', 'Name must be at least 2 characters');
    isValid = false;
  }
  
  // 2. Email validation (regex pattern matching)
  const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  if (!emailRegex.test(email)) {
    showError('emailError', 'Invalid email format');
    isValid = false;
  }
  
  // Return validation result
  return isValid;
}
```

**Algorithm Explanation**:
- **Type**: Sequential validation with early exit
- **Input**: Form field values (strings)
- **Output**: Boolean (true if valid, false otherwise)
- **Process**: 
  1. Initialize validation flag
  2. Clear previous error states
  3. Check each field sequentially
  4. Apply validation rules (required, length, format)
  5. Display errors if validation fails
  6. Return overall validation status

### 2. Smooth Scroll Algorithm

```javascript
/**
 * Implements smooth scrolling to target section
 * Algorithm: Calculated offset scroll with animation
 * Time Complexity: O(1) - constant time calculation
 */

function smoothScroll(targetElement) {
  const headerOffset = 80; // Fixed header height
  const elementPosition = targetElement.getBoundingClientRect().top;
  const offsetPosition = elementPosition + window.pageYOffset - headerOffset;
  
  window.scrollTo({
    top: offsetPosition,
    behavior: 'smooth'
  });
}
```

**Algorithm Explanation**:
- **Type**: Position calculation with animated scroll
- **Input**: Target DOM element
- **Output**: Window scroll action
- **Process**:
  1. Get target element's position relative to viewport
  2. Calculate absolute position on page
  3. Subtract header height for proper positioning
  4. Trigger smooth scroll animation

### 3. Intersection Observer (Scroll Animation)

```javascript
/**
 * Lazy animation trigger using Intersection Observer API
 * Algorithm: Observer pattern with threshold detection
 * Time Complexity: O(1) per observation
 */

const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      // Element is visible in viewport
      entry.target.style.opacity = '1';
      entry.target.style.transform = 'translateY(0)';
      
      // Stop observing (performance optimization)
      observer.unobserve(entry.target);
    }
  });
}, {
  threshold: 0.1, // Trigger when 10% visible
  rootMargin: '0px 0px -100px 0px' // Trigger slightly before
});
```

**Algorithm Explanation**:
- **Type**: Event-driven observer pattern
- **Data Structure**: Set of observed elements
- **Process**:
  1. Observer watches multiple DOM elements
  2. Triggers callback when element intersects viewport
  3. Applies CSS transformations for animation
  4. Unobserves element after animation (memory optimization)

### 4. Navigation Active State Algorithm

```javascript
/**
 * Highlights active navigation link based on scroll position
 * Algorithm: Linear search through sections
 * Time Complexity: O(n) where n = number of sections
 */

function highlightNavOnScroll() {
  const scrollY = window.pageYOffset;
  
  sections.forEach(section => {
    const sectionHeight = section.offsetHeight;
    const sectionTop = section.offsetTop - 100;
    const sectionId = section.getAttribute('id');
    
    // Check if current scroll position is within section
    if (scrollY > sectionTop && scrollY <= sectionTop + sectionHeight) {
      // Found active section
      const navLink = document.querySelector(`a[href="#${sectionId}"]`);
      navLink.classList.add('active');
    } else {
      // Remove active from other sections
      navLink.classList.remove('active');
    }
  });
}
```

**Algorithm Explanation**:
- **Type**: Linear search with range checking
- **Input**: Current scroll position
- **Output**: Updated navigation state
- **Process**:
  1. Get current scroll position
  2. Iterate through all sections
  3. Calculate section boundaries
  4. Check if scroll position falls within section
  5. Update active state accordingly

### Data Structures Used

#### 1. **DOM Tree**
```
Document
└── html
    ├── head
    │   ├── meta (viewport)
    │   ├── link (CSS files)
    │   └── title
    └── body
        ├── header
        │   └── nav
        │       ├── logo
        │       ├── ul (nav-links)
        │       └── burger
        ├── main
        │   ├── section (hero)
        │   ├── section (about)
        │   ├── section (skills)
        │   ├── section (projects)
        │   ├── section (experience)
        │   └── section (contact)
        └── footer
```

#### 2. **CSS Custom Properties (Hash Map)**
```javascript
// Conceptual representation
cssVariables = {
  '--primary-color': '#667eea',
  '--spacing-md': '1rem',
  '--font-size-xl': '1.25rem',
  // ...
}
```

**Benefits**:
- O(1) lookup time
- Single source of truth for design values
- Easy theming and maintenance

#### 3. **NodeList (Array-like)**
```javascript
const sections = document.querySelectorAll('section[id]');
// NodeList[section#home, section#about, section#skills, ...]

// Iteration: O(n)
sections.forEach(section => { /* ... */ });
```

---

## 🐛 Known Issues and Solutions

### Issue 1: Image Loading Delay
**Problem**: Project images load slowly on slow connections
**Solution**: Implemented lazy loading and image optimization
```html
<img loading="lazy" src="images/project.jpg" alt="Project">
```

### Issue 2: Mobile Menu Z-Index
**Problem**: Menu appeared behind certain elements
**Solution**: Proper z-index layering system
```css
:root {
  --z-sticky: 1020;
  --z-modal: 1040;
}
```

### Issue 3: Form Submission on GitHub Pages
**Problem**: No backend to handle form submissions
**Solution**: Integrated FormSpree third-party service
```html
<form action="https://formspree.io/f/xbdqdknj" method="POST">
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Akanksha Waghamode**

- 📧 Email: akankshawaghamode2001@gmail.com
- 📱 Phone: +91-8080640427
- 💼 LinkedIn: [Akanksha Waghamode](https://www.linkedin.com/in/akanksha-waghamode-25aa9724a/)
- 💻 GitHub: [@akanksha3-3](https://github.com/akanksha3-3)
- 📍 Location: Pune, Maharashtra, India

---

## 🙏 Acknowledgments

### Resources and Inspiration
- **CSS Tricks**: For CSS Grid and Flexbox tutorials
- **MDN Web Docs**: Comprehensive web development documentation
- **W3C**: HTML and CSS specifications and validators
- **Font Awesome**: Icon library
- **Unsplash & Pexels**: Free stock images
- **FormSpree**: Form backend service
- **GitHub Pages**: Free hosting service

---
