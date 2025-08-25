# Simple Personal Portfolio

A modern, responsive personal portfolio website built with HTML, Tailwind CSS, and JavaScript. Features dark/light mode toggle, smooth animations, and a clean design.
You can see the example on [Here!](https://dhitera.github.io/simple-personal-portfolio/)

## 🌟 Features

- **Responsive Design** - Works perfectly on desktop, tablet, and mobile
- **Dark/Light Mode** - Toggle between themes with a smooth transition
- **Smooth Animations** - AOS (Animate On Scroll) library for beautiful page transitions
- **Modern UI** - Clean, professional design with gradients and glass-morphism effects
- **Easy Customization** - Simple HTML structure for easy editing

## 🚀 Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm (comes with Node.js)

### Installation

1. **Clone or download this repository**

   ```bash
   git clone <repository-url>
   cd simple-personal-portfolio
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Build the CSS**

   ```bash
   npm run build
   ```

4. **Start development server (optional)**

   ```bash
   npm run dev
   ```

5. **Open the portfolio**
   - Open `index.html` in your web browser
   - Or use a local server like Live Server extension in VS Code

## 📝 Customization Guide

### 1. Personal Information

Edit the following sections in `index.html`:

#### Navigation Brand

```html
<span
  class="self-center text-3xl font-semibold whitespace-nowrap text-orange-500 font-serif dark:text-blue-700"
>
  Nickname
  <!-- Change this to your name/brand -->
</span>
```

#### Hero Section

```html
<p
  class="text-lg md:text-xl lg:text-2xl italic font-semibold text-gray-500 opacity-80 font-mono mt-2"
>
  Hello, my name is
  <!-- Update greeting -->
</p>
<p class="text-4xl md:text-6xl lg:text-7xl font-serif font-bold">
  Your
  <span class="text-orange-500 dark:text-blue-700">Name</span> Here
  <!-- Change to your actual name -->
</p>
<p
  class="text-lg md:text-xl lg:text-2xl font-semibold text-gray-500 opacity-80 font-mono mt-2 me-2 text-center md:text-right"
>
  Your Specialist / Field
  <!-- Change to your profession -->
</p>
```

#### Profile Image

Replace `img/profilePict.jpg` with your own image:

1. Add your photo to the `img/` folder
2. Update the src attribute:

```html
<img src="img/your-photo.jpg" alt="Profile image" ... />
```

### 2. About Section

#### About Text

```html
<p
  class="mt-2 text-base md:text-lg lg:text-xl text-center font-sans max-w-4xl mx-auto"
>
  <!-- Replace with your personal description -->
  Write about yourself, your background, interests, and what you do...
</p>
```

#### Skills

Update the skill badges:

```html
<span
  class="text-white text-sm md:text-lg font-medium px-3 py-1.5 rounded-full bg-gradient-to-r from-orange-300 to-orange-600 dark:from-blue-600 dark:to-purple-700"
  data-aos="fade-up"
  data-aos-duration="700"
>
  Your Skill Here
  <!-- Replace with your actual skills -->
</span>
```

### 3. Experience Section

Replace the dummy experience entries with your own:

```html
<li class="mb-10 ms-4">
  <div
    class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"
  ></div>
  <div data-aos="fade-down" data-aos-duration="700">
    <time
      class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500"
    >
      Your Date Range
      <!-- e.g., Jan 2023 - Present -->
    </time>
    <h3 class="text-lg font-semibold text-gray-900 dark:text-white">
      Your Job Title
      <!-- e.g., Senior Developer -->
    </h3>
    <p class="text-base font-bold text-orange-500 dark:text-blue-400">
      Company Name
      <!-- e.g., Tech Company Inc. -->
    </p>
    <ul
      class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400 list-disc list-inside"
    >
      <li>Your achievement or responsibility 1</li>
      <li>Your achievement or responsibility 2</li>
      <li>Your achievement or responsibility 3</li>
    </ul>
  </div>
</li>
```

### 4. Gallery Section

The gallery uses placeholder images from Picsum. To use your own images:

1. Add your images to the `img/` folder
2. Replace the image sources:

```html
<img
  class="w-full h-64 object-cover rounded-lg"
  src="img/your-image.jpg"
  alt="Your Description"
/>
```

3. Update the gallery description:

```html
<p
  class="text-lg md:text-xl text-gray-700 dark:text-gray-200 italic font-serif"
>
  Your gallery description here
</p>
```

### 5. Contact Information

Update your contact details:

```html
<!-- Email -->
<a href="mailto:your-email@example.com" target="_blank">
  <a href="mailto:your-email@example.com" target="_blank" class="...">
    your-email@example.com
  </a>

  <!-- Instagram -->
  <a href="https://www.instagram.com/your-username" target="_blank">
    <a
      href="https://www.instagram.com/your-username"
      target="_blank"
      class="..."
    >
      @your-username
    </a>

    <!-- LinkedIn -->
    <a href="https://www.linkedin.com/in/your-profile" target="_blank">
      <a
        href="https://www.linkedin.com/in/your-profile"
        target="_blank"
        class="..."
      >
        your-profile
      </a></a
    ></a
  ></a
>
```

### 6. Footer

Update the copyright information:

```html
<p class="text-sm text-gray-600 dark:text-gray-400">
  © 2025
  <span class="text-orange-500 dark:text-blue-400 font-semibold"
    >Your Name</span
  >
  . All rights reserved.
</p>
```

## 🎨 Customizing Colors

The portfolio uses a orange/blue color scheme. To change colors, update these Tailwind classes:

### Light Mode Colors

- Primary: `orange-300`, `orange-500`, `orange-600`, `amber-600`
- Accent: `orange-500`

### Dark Mode Colors

- Primary: `blue-600`, `blue-700`, `purple-700`
- Accent: `blue-700`

### Example Color Changes

```html
<!-- Change from orange to purple -->
<span class="text-purple-500 dark:text-green-700">Name</span>

<!-- Change gradient colors -->
<div
  class="bg-gradient-to-r from-purple-300 to-purple-600 dark:from-green-600 dark:to-teal-700"
></div>
```

## 📱 Adding More Sections

To add new sections, follow this structure:

```html
<section
  id="new-section"
  class="bg-slate-50 dark:bg-gray-900 py-10 px-4 md:px-15 min-h-screen"
>
  <div class="max-w-screen-xl mx-auto">
    <div class="text-center mb-8" data-aos="fade-in">
      <h2
        class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 dark:text-white underline decoration-amber-600 dark:decoration-indigo-500 underline-offset-8"
      >
        Section Title
      </h2>
    </div>
    <!-- Your content here -->
  </div>
</section>
```

Don't forget to add the navigation link:

```html
<li>
  <a href="#new-section" class="block py-2 px-3 text-gray-400 ... ">
    Section Name
  </a>
</li>
```

## 🛠️ Available Scripts

- `npm run build` - Build the Tailwind CSS
- `npm run dev` - Start development mode with file watching
- `npm run watch` - Watch for changes and rebuild CSS

## 📦 Dependencies

- **Tailwind CSS** - Utility-first CSS framework
- **AOS** - Animate On Scroll library
- **Flowbite** - Tailwind CSS components

## 🤝 Contributing

Feel free to fork this project and customize it for your own use. If you make improvements, consider sharing them!

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy coding!** 🚀 Make this portfolio template your own and showcase your amazing work to the world.
