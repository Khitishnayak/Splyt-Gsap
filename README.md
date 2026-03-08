# SPYLT — Animated Landing Page

A fully animated, scroll-driven marketing landing page for **SPYLT**, a protein + caffeine drink brand. Built with React, GSAP, and Tailwind CSS.

## ✨ Features

- **Smooth scrolling** powered by GSAP ScrollSmoother
- **Scroll-triggered animations** with GSAP ScrollTrigger across every section
- **Character & word split-text animations** using GSAP SplitText
- **Clip-path reveal animations** for titles and cards
- **Interactive flavor slider** showcasing all six SPYLT flavors
- **Pinned video section** highlighting product benefits
- **Testimonial cards** with rotated video clips
- **Fully responsive** layout supporting mobile, tablet, and desktop (via `react-responsive`)

## 🏗️ Tech Stack

| Technology | Purpose |
|---|---|
| [React 19](https://react.dev/) | UI component library |
| [Vite](https://vite.dev/) | Build tool and dev server |
| [GSAP](https://gsap.com/) + [@gsap/react](https://gsap.com/docs/v3/Packages/@gsap/react/) | Animations (ScrollTrigger, ScrollSmoother, SplitText) |
| [Tailwind CSS v4](https://tailwindcss.com/) | Utility-first styling |
| [react-responsive](https://github.com/yocontra/react-responsive) | Responsive breakpoint hooks |

## 📄 Page Sections

1. **NavBar** — Fixed navigation bar
2. **Hero** — Full-screen intro with split-text title animation and scroll rotation effect
3. **Message** — Brand message reveal section
4. **Flavors** — Interactive slider for all six flavors: Chocolate Milk, Strawberry Milk, Cookies & Cream, Peanut Butter Chocolate, Vanilla Milkshake, and Max Chocolate Milk
5. **Nutrition** — Nutrient breakdown (Potassium, Calcium, Vitamin A, Vitamin D, Iron) with scroll-triggered animations
6. **Benefits** — Clip-path animated benefit titles (Shelf Stable, Protein + Caffeine, Infinitely Recyclable, Lactose Free) with a pinned video
7. **Testimonials** — Rotated video testimonial cards
8. **Footer** — Social links, newsletter signup, and site navigation

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- npm v9 or higher

> **Note:** This project uses GSAP premium plugins (ScrollSmoother, SplitText). You will need a valid [GSAP Club](https://gsap.com/pricing/) membership or trial license to use these features.

### Installation

```bash
# Clone the repository
git clone https://github.com/Khitishnayak/Splyt-Gsap.git
cd Splyt-Gsap

# Install dependencies
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production Build

```bash
npm run build
```

Built files are output to the `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

### Lint

```bash
npm run lint
```

## 📁 Project Structure

```
Splyt-Gsap/
├── public/
│   ├── fonts/          # Custom font files
│   ├── images/         # Static images and icons
│   └── videos/         # Background and testimonial videos
├── src/
│   ├── components/     # Reusable UI components
│   │   ├── ClipPathTitle.jsx
│   │   ├── FlavorSlider.jsx
│   │   ├── FlavorTitle.jsx
│   │   ├── NavBar.jsx
│   │   └── VideoPinSection.jsx
│   ├── constants/
│   │   └── index.js    # Shared data (flavors, nutrients, testimonial cards)
│   ├── sections/       # Full-page sections
│   │   ├── HeroSection.jsx
│   │   ├── MessageSection.jsx
│   │   ├── FlavorSection.jsx
│   │   ├── NutritionSection.jsx
│   │   ├── BenefitSection.jsx
│   │   ├── TestimonialSection.jsx
│   │   └── FooterSection.jsx
│   ├── App.jsx         # Root component, GSAP plugin registration
│   ├── index.css       # Global styles
│   └── main.jsx        # React entry point
├── index.html
├── vite.config.js
├── eslint.config.js
└── package.json
```
