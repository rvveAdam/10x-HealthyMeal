# HealthyMeal

A web application that allows users to customize recipes according to their personal needs and dietary preferences with AI assistance.

## Project Description

HealthyMeal is a browser application that enables users to browse recipes, modify ingredients with AI assistance, add their own recipes, and filter available dishes based on various criteria. The application helps users adapt recipes to their specific dietary needs while maintaining flavor and nutritional value.

### Main Features
- User account system with full management (registration, login, edit, delete)
- Recipe catalog from a dedicated database and ability to add your own recipes
- Intelligent recipe modifications with ingredient substitute suggestions
- Advanced recipe filtering by preferences (sweet/savory, calorie content, difficulty level)
- Recipe rating system on a 1-5 star scale

## Tech Stack

- [Astro](https://astro.build/) v5.5.5 - Modern web framework for building fast, content-focused websites
- [React](https://react.dev/) v19.0.0 - UI library for building interactive components
- [TypeScript](https://www.typescriptlang.org/) v5 - Type-safe JavaScript
- [Tailwind CSS](https://tailwindcss.com/) v4.0.17 - Utility-first CSS framework
- [Shadcn/ui](https://ui.shadcn.com/) - Accessible React component library
- [Supabase](https://supabase.com/) - Backend-as-a-Service providing PostgreSQL database and authentication
- [OpenRouter.ai](https://openrouter.ai/) - AI model access for ingredient substitution features

## Getting Started Locally

### Prerequisites

- Node.js v22.14.0 (as specified in `.nvmrc`)
- npm (comes with Node.js)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/healthymeal.git
cd healthymeal
```

2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file based on the provided `.env.example` template and fill in the required environment variables.

4. Run the development server:

```bash
npm run dev
```

5. Open your browser and navigate to `http://localhost:4321` to see the application.

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run astro` - Run Astro CLI commands
- `npm run lint` - Run ESLint
- `npm run lint:fix` - Fix ESLint issues
- `npm run format` - Format code with Prettier

## Project Scope

### What the Product Will Do
- Enable user account management
- Present a recipe catalog with filtering options
- Allow recipe modification and suggest ingredient substitutes
- Let users add their own recipes (limited to 5 per user)
- Provide a recipe rating system
- Work as a browser application with responsive design

### What the Product Will Not Do
- No user notifications
- No ability to add more than 5 custom recipes per user
- No editing of entire recipes, only ingredients
- No social features (recipe sharing, commenting, etc.)
- No mobile app (only responsive website)
- No information about ingredient availability in stores
- No multi-day meal planning

## Project Status

This project is currently in development. The initial version focuses on core functionality including:

- User authentication and profile management
- Basic recipe browsing and filtering
- AI-powered ingredient substitution
- Custom recipe addition
- Recipe rating system

Future updates may include more advanced filtering options, additional AI features, and improved user experience based on feedback and metrics.

## License

MIT
