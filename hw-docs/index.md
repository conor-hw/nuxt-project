# Nuxt Project Documentation

This is the documentation for the Nuxt RealWorld Example App.

It demonstrates a fully fledged fullstack application built with Nuxt3, including CRUD operations, authentication, routing, pagination, and more. The application adheres to the RealWorld specification, providing a standard an exemplary way to build real-world applications with Nuxt 3.

## Key Aspects

- **Nuxt 3 Framework:** Leverages the latest features of Nuxt 3 for server-side rendering (SSR), static site generation (SSG), and client-side rendering (CSR).
- **RealWorld Spec Adherence:** Follows the RealWorld project specifications, showcasing a practical, real-world application.
- **Best Practices:** Demonstrates best practices for Nuxt 3 development, including project structure, state management, and component design.
- **Fullstack Capabilities:** Includes features common in fullstack applications like user authentication, CRUD operations for articles, user profiles, and commenting.

## Technical Stack

The project is built with a modern and robust technical stack:

- **Frontend Framework:** Nuxt 3 (using Vue 3)
- **UI Framework:** Quasar UI, providing a rich set of pre-built components.
- **State Management:** Likely Nuxt 3's built-in composables or Pinia (though not explicitly confirmed, common for Nuxt 3).
- **Styling:** SCSS for styling, with global styles and Quasar variable overrides.
- **API Interaction:** Uses runtime configurations (`baseUrl`) for connecting to a backend API.
- **Markdown Processing:** Utilizes `marked` for rendering Markdown content and `sanitize-html` for security.
- **Development Tools:**
    - TypeScript for static typing.
    - ESLint and Prettier for code linting and formatting.
    - Husky for Git hooks to enforce code quality.
    - Nuxt Devtools for an enhanced development experience.

## Project Structure Overview

The project follows a standard Nuxt 3 structure:

- **`assets/`**: Contains uncompiled assets like stylesheets (SCSS) and images.
- **`components/`**: Houses reusable Vue components.
- **`composables/`**: For Nuxt 3's auto-imported composable functions (Vue 3 Composition API).
- **`constants/`**: Likely holds application-wide constants.
- **`layouts/`**: Defines the different layouts for pages (e.g., default, authenticated).
- **`middleware/`**: Contains route middleware for tasks like authentication checks.
- **`pages/`**: Defines the application's routes and views.
- **`public/`**: Stores static assets that are directly served.
- **`server/`**: For server-side API routes or middleware, if any are defined within the Nuxt app itself.
- **`services/`**: Likely contains logic for interacting with external APIs.
- **`store/`**: For state management (e.g., Pinia stores).
- **`types/`**: Holds TypeScript type definitions.
- **`utils/`**: Contains utility functions.
- **`nuxt.config.ts`**: The main configuration file for Nuxt.
- **`package.json`**: Lists project dependencies and scripts.

## How it Works

The application functions as a "Conduit" clone, a platform for sharing articles. Here's a high-level overview:

1.  **User Interface:** The frontend is built with Nuxt 3 and Quasar UI, providing a reactive and modern user experience.
2.  **Routing:** Nuxt 3's file-system based routing handles navigation between different pages like the home feed, article details, user profiles, and settings.
3.  **Authentication:** Users can register and log in. Authentication status is likely managed using cookies (as hinted by `cookieName` in `nuxt.config.ts`) and route middleware to protect certain routes.
4.  **API Interaction:** The application interacts with a backend API (specified by `baseUrl`) to fetch and submit data for articles, comments, user profiles, and authentication.
5.  **State Management:** Application state (e.g., current user, articles) is managed, likely using Nuxt 3's built-in reactivity or a dedicated state management library like Pinia.
6.  **Content Display:** Articles, potentially written in Markdown, are processed and displayed.

This project serves as a comprehensive example of building a feature-rich web application with Nuxt 3, showcasing its capabilities and development patterns.
