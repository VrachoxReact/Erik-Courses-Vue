# Erik-Courses-Vue

A modern, responsive web application for a boxing academy offering online courses. This project is built using Vue.js, TypeScript, and Tailwind CSS.

## Features

- **Course Catalog**: Browse and filter courses by category, level, and price
- **Course Details**: Detailed information about each course, including curriculum and reviews
- **Shopping Cart**: Add courses to cart, apply discount codes, and proceed to checkout
- **User Authentication**: Register, log in, and manage user accounts
- **Responsive Design**: Optimized for all device sizes, from mobile to desktop

## Tech Stack

- Vue 3 with Composition API
- TypeScript
- Vite for build tooling
- Vue Router for navigation
- Pinia for state management
- Tailwind CSS for styling
- Element Plus UI components
- Heroicons for icons

## Project Structure

```
src/
├── assets/          # Static assets (images, etc.)
├── components/      # Reusable Vue components
│   └── layout/      # Layout components (Header, Footer)
├── router/          # Vue Router configuration
├── stores/          # Pinia stores
│   ├── cartStore.ts # Shopping cart state
│   ├── courseStore.ts # Course data and operations
│   ├── userStore.ts # User authentication and profile
│   └── uiStore.ts   # UI state (notifications, etc.)
├── views/           # Page components
│   ├── AboutView.vue
│   ├── AccountView.vue
│   ├── AuthView.vue
│   ├── CartView.vue
│   ├── CheckoutView.vue
│   ├── ContactView.vue
│   ├── CourseDetailView.vue
│   ├── CoursesView.vue
│   ├── HomeView.vue
│   └── NotFoundView.vue
├── App.vue          # Root component
├── main.ts          # Application entry point
└── style.css        # Global styles
```

## Getting Started

### Prerequisites

- Node.js 20.x or later (required by Vite 6.x and other dependencies)
- npm or yarn

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/VrachoxReact/Erik-Courses-Vue.git
   cd Erik-Courses-Vue
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npm run dev
   ```

4. Build for production
   ```bash
   npm run build
   ```

## Deployment to Vercel

This project is configured for easy deployment to Vercel:

1. Push your code to GitHub
   ```bash
   git add .
   git commit -m "Ready for deployment"
   git push
   ```

2. Connect to Vercel:
   - Go to [Vercel.com](https://vercel.com) and sign up/log in
   - Click "Add New" → "Project"
   - Connect to your GitHub repository
   - Vercel will automatically detect it's a Vue/Vite project

3. Configuration:
   - Vercel will automatically detect the correct build settings
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`
   - Development Command: `npm run dev`

4. After deployment, you can:
   - Configure a custom domain
   - Enable HTTPS
   - Set up environment variables if needed
   - Configure project settings through the Vercel dashboard

## Development

### Adding New Courses

Add new courses by extending the course data in `src/stores/courseStore.ts`.

### Modifying Styles

This project uses Tailwind CSS. Customize the theme in `tailwind.config.js`.

## License

MIT

## Acknowledgements

- Erik Pijetraj for the boxing expertise
- Icons provided by [Heroicons](https://heroicons.com/)
- UI components from [Element Plus](https://element-plus.org/)