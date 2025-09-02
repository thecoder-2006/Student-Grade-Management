# Overview

This is a student grade card management system built as a full-stack web application. The system allows users to view, add, edit, delete, and search student records with their marks and calculated grades. The application features a modern React frontend with TypeScript and a Node.js/Express backend, using SQLite for local data storage with Drizzle ORM for database operations.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript using Vite as the build tool
- **UI Library**: Shadcn/ui components built on Radix UI primitives with Tailwind CSS for styling
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query (React Query) for server state management and API caching
- **Form Handling**: React Hook Form with Zod validation schemas
- **Styling**: Tailwind CSS with CSS variables for theming support

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database**: SQLite with better-sqlite3 driver for local file-based storage
- **ORM**: Drizzle ORM for type-safe database operations
- **API**: RESTful endpoints for CRUD operations on student data
- **Development**: Vite integration for hot module replacement in development

## Data Storage
- **Database**: SQLite file-based database (`students.db`)
- **Schema**: Single `students` table with id, name, marks, and calculated grade fields
- **Grade Calculation**: Automatic grade assignment based on marks (A+ ≥90, A ≥80, B ≥70, C ≥60, D ≥50, F <50)
- **Sample Data**: Pre-populated with 10 sample student records on first run

## Key Features
- **CRUD Operations**: Create, read, update, delete student records
- **Search & Filter**: Search by student name and filter by grade
- **Grade Statistics**: Visual distribution of grades with color-coded indicators
- **Responsive Design**: Mobile-first approach with adaptive layouts
- **Form Validation**: Client-side validation with Zod schemas
- **Error Handling**: Comprehensive error handling with user-friendly toast notifications

## Project Structure
- `/client` - React frontend application
- `/server` - Express backend with API routes and database logic
- `/shared` - Shared TypeScript types and validation schemas
- Component organization follows atomic design with reusable UI components

# External Dependencies

## Core Framework Dependencies
- **React & TypeScript**: Frontend framework with type safety
- **Express.js**: Backend web framework for Node.js
- **Vite**: Build tool and development server

## Database & ORM
- **better-sqlite3**: Synchronous SQLite driver for Node.js
- **Drizzle ORM**: Type-safe ORM with migration support
- **Drizzle-Zod**: Integration between Drizzle and Zod for schema validation

## UI & Styling
- **Radix UI**: Headless UI component primitives
- **Tailwind CSS**: Utility-first CSS framework
- **Shadcn/ui**: Pre-built component library
- **Lucide React**: Icon library

## Form & Validation
- **React Hook Form**: Form state management
- **Zod**: Schema validation library
- **@hookform/resolvers**: Integration between React Hook Form and Zod

## State Management
- **TanStack Query**: Server state management and caching
- **Wouter**: Lightweight client-side routing

## Development Tools
- **TypeScript**: Static type checking
- **ESLint & Prettier**: Code linting and formatting
- **PostCSS**: CSS processing with Tailwind integration