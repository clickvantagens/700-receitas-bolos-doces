# Overview

This is a landing page application for a Brazilian recipe collection product ("700 receitas"). It's built as a full-stack web application using React for the frontend and Express.js for the backend, with a focus on marketing and sales conversion. The application appears to be designed for selling a digital recipe collection with payment integration through platforms like Kiwify.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript and Vite as the build tool
- **UI Library**: Shadcn/ui components built on Radix UI primitives for accessibility
- **Styling**: Tailwind CSS with custom design tokens and CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Forms**: React Hook Form with Zod validation resolvers

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM configured for PostgreSQL
- **Session Management**: Express sessions with PostgreSQL session store (connect-pg-simple)
- **Development**: Hot reload with Vite integration in development mode

## Component System
- **Design System**: Consistent component library using class-variance-authority for variant management
- **Accessibility**: Built on Radix UI primitives ensuring WCAG compliance
- **Theming**: CSS custom properties with automatic dark/light mode support
- **Icons**: Lucide React for consistent iconography

## Build and Development
- **Development Server**: Vite dev server with HMR and error overlay
- **Build Process**: Vite for frontend bundling, esbuild for backend compilation
- **Type Checking**: Shared TypeScript configuration across client/server/shared modules
- **Code Organization**: Monorepo structure with shared types and utilities

## Data Layer
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema**: Centralized schema definitions in shared directory
- **Migrations**: Drizzle Kit for database migration management
- **Environment**: Environment-based database URL configuration

# External Dependencies

## Database Services
- **PostgreSQL**: Primary database (configured for Neon Database serverless)
- **Connection**: @neondatabase/serverless for serverless PostgreSQL connections

## Payment Integration
- **Kiwify**: Payment processor for digital product sales (configured in landing page)
- **WhatsApp Business API**: Customer communication integration

## Development Tools
- **Replit**: Development environment with specific cartographer and error modal plugins
- **Vite Plugins**: Runtime error overlay and development banner for Replit environment

## UI and Design
- **Google Fonts**: Inter font family for typography
- **Unsplash**: Image hosting for product photography and marketing materials
- **Radix UI**: Comprehensive primitive component library for accessibility

## Frontend Libraries
- **TanStack Query**: Server state management and caching
- **React Hook Form**: Form handling and validation
- **Zod**: Runtime type validation and schema definition
- **Date-fns**: Date manipulation and formatting utilities
- **Embla Carousel**: Carousel/slider functionality for image galleries