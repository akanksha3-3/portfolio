# Personal Portfolio Website - Akanksha Waghamode

## 📋 Project Overview

### Project Description
A fully responsive personal portfolio website designed to showcase my skills, projects, and professional experience in Data Science and Bioinformatics. This project demonstrates proficiency in modern web development technologies and follows industry-standard best practices for responsive design, accessibility, and user experience.

## 🚀 Live Portfolio
👉 https://akanksha3-3.github.io/portfolio/

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

###  Performance Testing

#### Load Time Analysis (Desktop):
- **First Contentful Paint**: 0.6s
- **Largest Contentful Paint**: 0.6s
- **Total Blocking Time**: 0 ms
- **Cumulative Layout Shift**: 0
- **Speed Index**: 0.9s

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
