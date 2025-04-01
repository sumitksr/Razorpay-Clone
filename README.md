# Razorpay Website Clone



A fully responsive clone of the Razorpay website built with HTML, CSS, and JavaScript. This project focuses on recreating Razorpay's modern UI with interactive elements using TailwindCSS.

## 🚀 Features

- **Pixel-perfect UI** matching the original Razorpay website
- **Fully responsive** design that works on mobile, tablet, and desktop
- **Interactive navigation** with animated dropdown menus
- **Optimized images** for faster loading
- **Modern animations** for an engaging user experience
- **Clean, well-structured code** following best practices

## 🔧 Technologies Used

- **HTML5** - For structure and semantic markup
- **TailwindCSS** - For styling and responsive design
- **JavaScript** - For interactivity and animations
- **Feather Icons** - For lightweight, consistent icons

## 📋 Key Sections

1. **Hero Section** - Main banner with call-to-action
2. **Payment Features** - Showcasing Razorpay's payment solutions
3. **Banking Section** - Highlighting Razorpay Banking services
4. **Product Features** - Displaying various product offerings
5. **Core Features** - Detailed feature explanation
6. **Testimonials** - Customer reviews and experiences
7. **CTA Section** - Final call-to-action
8. **Footer** - Comprehensive site navigation

## 💡 Interactive Elements

### Navigation Bar
- **Animated Dropdowns** - Smooth transitions and animations
- **Hover Effects** - Visual feedback for better user experience
- **Mobile-Responsive** - Adaptable to various screen sizes

### Feature Cards
- **Hover Animations** - Elements transform on hover
- **Visual Feedback** - Color changes and shadow effects
- **Staggered Animations** - Sequential appearance for dropdown items

## 🧠 Interactive Navbar Implementation

The interactive navigation bar is one of the standout features of this project, implementing complex dropdown menus with pure CSS:

### Technical Details

- **CSS-only Implementation** - No JavaScript required for the dropdown functionality
- **Group Hover States** - Using TailwindCSS's group hover mechanism to trigger dropdown visibility
- **Custom Animation Keyframes** - Defined custom animations for smooth transitions
- **Z-Index Management** - Careful layering to prevent overlap issues
- **Pseudo-elements** - Used for creating hover indicators and transitions

### Animation Specifications

```css
/* Fade-in animation for dropdowns */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Staggered animation for menu items */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-10px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}
```

### Dropdown Structure

Each dropdown menu follows this structure:
1. **Parent List Item** - Contains the main navigation link
2. **Dropdown Container** - Positioned absolutely with initial `opacity: 0` and `invisible`
3. **Group Hover Controls** - Show the dropdown using `group-hover:opacity-100` and `group-hover:visible`
4. **Content Sections** - Organized content with headers, icons, and descriptions
5. **Item Hover Effects** - Individual hover states for each dropdown item

### Accessibility Considerations

- **High Contrast Colors** - Ensuring text is readable against backgrounds
- **Logical Tab Order** - Maintaining proper navigation flow
- **Hover and Focus States** - Visual indicators for interactive elements
- **Semantic HTML** - Using appropriate elements for proper screen reader interpretation

## 📂 Project Structure

```
razorpay-clone/
├── index.html          # Main HTML file
├── main.css            # TailwindCSS output
├── README.md           # Project documentation
└── Images/             # Image assets
    ├── logo.svg
    ├── hero-illustration.jpg
    ├── feature-section1-dottedrows.png
    └── ...
```

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/username/razorpay-clone.git
   cd razorpay-clone
   ```

2. **Open the project**
   ```bash
   # Simply open index.html in your browser
   # For VS Code users
   code .
   ```

3. **View the website**
   - Open `index.html` in your preferred browser
   - No build process required!

## ⚙️ TailwindCSS Configuration

This project uses TailwindCSS for styling. The configuration is minimal but effective:

### Setup

If you want to modify the TailwindCSS configuration:

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Configure TailwindCSS**
   The `tailwind.config.js` file contains customizations:

   ```javascript
   module.exports = {
     content: ["./*.html"],
     theme: {
       extend: {
         colors: {
           deepBlue: "#02042a",
           lightBlue: "#2b84ea",
           lightBlue300: "#4b94ed",
           lightBlue500: "#0b72e7",
           greenLight: "#61cea6",
           grayText: "#818597",
           lightGray: "#e2e2e2",
           grayBlue: "#344a6c",
           deepBlueHead: "#162f56",
           gray2: "#525a76",
         },
         fontFamily: {
           mullish: ["Mulish", "sans-serif"],
         },
       },
     },
     plugins: [],
   };
   ```

3. **Compile CSS**
   ```bash
   # Development mode
   npm run dev
   
   # Production build
   npm run build
   ```

### Custom Classes

The project also uses custom utility classes for specific components:

```css
/* Example of custom utility classes */
.featureCard:hover .featureCardIcon {
  background-image: linear-gradient(
    30.55deg,
    #6ac7ff 11.05%,
    #148aff 90.09%
  );
  box-shadow: 0px 2px 22px rgb(202 202 202 / 25%);
}

.coreFeature {
  background-size: 100% 100%;
  padding-top: 14rem;
  padding-bottom: 12rem;
}
```

## 🧩 Key Implementation Details

### TailwindCSS Integration
The project uses TailwindCSS for styling, with custom utility classes for specific design elements.

### Interactive Navigation
The navbar features custom-built dropdown menus with smooth animations and transitions:
- Fade-in animations
- Hover effects
- Sequential item appearance
- Dynamic positioning

### Custom Animations
Several custom animations are implemented:
- Card hover effects
- Staggered animations
- Scroll-triggered animations
- Transition effects

## 🧪 Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## 🌟 Future Improvements

- Add more interactive elements
- Implement dark mode
- Add form validation for contact forms
- Create additional pages for complete site experience
- Optimize further for performance

## 📊 Performance Optimization

This project implements several performance optimization techniques:

### Image Optimization

- **Lazy Loading** - Images use the `loading="lazy"` attribute to defer loading until needed
- **Appropriate Sizing** - Images are sized appropriately for their containers
- **Image Formats** - SVG used for icons and logos for better scaling
- **Width/Height Attributes** - Explicit dimensions to prevent layout shifts

### CSS Optimization

- **TailwindCSS Purging** - Unused CSS is removed in production builds
- **Minimal Custom CSS** - Custom styles only where necessary
- **CSS Organization** - Styles are organized by component for better maintainability
- **Critical CSS** - Essential styles are included inline in the head

### Code Optimization

- **Minimal JavaScript** - Primarily using CSS for animations and interactions
- **Deferred Script Loading** - Non-essential scripts load after page render
- **Code Splitting** - Features organized into logical components
- **SVG Optimization** - SVGs optimized for size and performance

## 📱 Responsive Design

The project is fully responsive across all device sizes:

### Mobile First Approach

The design adopts a mobile-first approach with progressive enhancement for larger screens:

- **Fluid Typography** - Text scales appropriately across device sizes
- **Responsive Grid** - TailwindCSS grid system adapts to different screens
- **Breakpoint Strategy** - Carefully chosen breakpoints for optimal layouts
- **Component Adaptation** - Components transform based on available space

### Key Breakpoints

```css
/* Key breakpoints used in this project */
sm: '640px',   /* Small devices (phones) */
md: '768px',   /* Medium devices (tablets) */
lg: '1024px',  /* Large devices (laptops) */
xl: '1280px',  /* Extra large devices (desktops) */
```

### Responsive Components

- **Navigation** - Transforms from dropdown menu to hamburger menu on mobile
- **Feature Cards** - Adjust from multi-column to single column layout
- **Hero Section** - Adapts content and image placement for different screens
- **Footer** - Reorganizes links and sections for better mobile experience

### Testing

Responsive design has been tested on:
- Mobile devices (320px - 480px)
- Tablets (481px - 768px)
- Laptops (769px - 1024px)
- Desktops (1025px and above)

