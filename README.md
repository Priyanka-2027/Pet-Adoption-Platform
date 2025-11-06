# Pet Adoption Platform - Frontend

A modern, responsive web application built with React, TypeScript, and Vite, designed to connect pets in need with loving homes.

## 🚀 Features

- **Pet Browsing**: View available pets with detailed profiles
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Built with shadcn/ui components and Tailwind CSS
- **State Management**: Utilizes React Query for efficient data fetching and caching
- **Form Handling**: Robust form validation with React Hook Form and Zod
- **Theming**: Supports light/dark mode
- **Animations**: Smooth UI interactions with Framer Motion
- **Accessibility**: Built with a11y in mind using Radix UI primitives

## 🛠 Tech Stack

- **Framework**: React 18
- **Language**: TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS + shadcn/ui
- **State Management**: React Query
- **Form Handling**: React Hook Form + Zod
- **Routing**: React Router v6
- **UI Components**: Radix UI Primitives + shadcn/ui
- **Icons**: Lucide React
- **Date Handling**: date-fns
- **Charts**: Recharts
- **Carousel**: Embla Carousel
- **Toasts**: Sonner

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd pet-adoption-platform
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn
   # or
   pnpm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the project root and add the necessary environment variables:
   ```env
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

## 🚀 Development

1. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

2. **Build for production**
   ```bash
   npm run build
   # or
   yarn build
   # or
   pnpm build
   ```

3. **Preview production build**
   ```bash
   npm run preview
   # or
   yarn preview
   # or
   pnpm preview
   ```

## 📁 Project Structure

```
src/
├── assets/          # Static assets (images, fonts, etc.)
├── components/      # Reusable UI components
├── contexts/        # React context providers
├── hooks/           # Custom React hooks
├── lib/             # Utility functions and configurations
├── pages/           # Page components
├── styles/          # Global styles and Tailwind config
└── types/           # TypeScript type definitions
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [shadcn/ui](https://ui.shadcn.com/) for the beautiful component library
- [Tailwind CSS](https://tailwindcss.com/) for utility-first CSS
- [Vite](https://vitejs.dev/) for the amazing build tooling
- [React Query](https://tanstack.com/query) for server state management



# PawMatch Backend Overview

This document provides an overview of the key components and services that power the PawMatch application's backend. The backend is built using Supabase, which provides a PostgreSQL database, authentication, and serverless functions.

---

## Core Components

### 1. Database (PostgreSQL)
- **Purpose:** Stores all application data including users, pets, and adoption records.
- **Key Tables:**
  - `users`: Stores user account information.
  - `pets`: Contains details about pets available for adoption.
  - `wishlist`: Tracks pets saved by users.
  - `adoptions`: Manages the adoption application process.
  - `shelters`: Information about pet shelters and organizations.

### 2. Authentication
- **Purpose:** Handles user registration, login, and session management.
- **Features:**
  - Email/password authentication
  - Social logins (Google, GitHub, etc.)
  - JWT token management
  - Role-based access control (users, admins)

### 3. API Endpoints
- **Purpose:** Provides RESTful endpoints for frontend communication.
- **Key Endpoints:**
  - `/api/pets`: CRUD operations for pet listings
  - `/api/users`: User profile management
  - `/api/wishlist`: Manage user wishlists
  - `/api/adoptions`: Handle adoption applications
  - `/api/admin/*`: Admin-specific operations

### 4. Storage
- **Purpose:** Manages file uploads including pet images and documents.
- **Features:**
  - Secure file storage with access control
  - Image optimization and resizing
  - Public/private file access management

### 5. Serverless Functions
- **Purpose:** Handles complex business logic and third-party integrations.
- **Key Functions:**
  - AI-powered pet matching
  - Email notifications
  - Background processing
  - Data export/import

### 6. Real-time Subscriptions
- **Purpose:** Enables real-time updates across the application.
- **Use Cases:**
  - New pet listings
  - Adoption status updates
  - Wishlist notifications
  - Admin alerts

---

## Integration Points

### 1. Frontend Communication
- Secure API endpoints for data retrieval and updates
- WebSocket connections for real-time features
- File upload/download handling

### 2. Third-party Services
- Payment processing for adoption fees
- Email service for notifications
- AI/ML services for pet matching
- Analytics and monitoring tools

### 3. Security
- Row-level security (RLS) policies
- Rate limiting and abuse prevention
- Data validation and sanitization
- Regular security audits and updates

---

## Deployment & Operations

### 1. Infrastructure
- Hosted on Supabase
- Automatic scaling
- Daily backups
- Monitoring and alerting

### 2. CI/CD
- Automated testing
- Zero-downtime deployments
- Environment management (dev, staging, production)
- Rollback capabilities

### 3. Performance
- Database indexing and query optimization
- Caching strategies
- Asset optimization
- Load testing

---

This overview provides a comprehensive look at the backend architecture powering the PawMatch application, ensuring scalability, security, and performance for all users.


output screenshots:
frontend:
<img width="940" height="432" alt="image" src="https://github.com/user-attachments/assets/dfcc5a49-f1f4-4cfd-922a-1f8eb17d353f" />
<img width="951" height="662" alt="image" src="https://github.com/user-attachments/assets/b37f39ca-a7d3-4e9b-a9ff-cddd022ee485" />
<img width="940" height="395" alt="image" src="https://github.com/user-attachments/assets/7fba8f09-cf3c-499a-99b8-b23cde6233c3" />
<img width="940" height="401" alt="image" src="https://github.com/user-attachments/assets/fa024b6a-dbc3-426f-894b-396a79d1ac1d" />
<img width="940" height="540" alt="image" src="https://github.com/user-attachments/assets/c9446c9c-31bc-42e5-b4a1-a103177a1c7b" />
<img width="599" height="618" alt="image" src="https://github.com/user-attachments/assets/840b391c-ee32-42c1-b5dd-7b1b414ae49a" />
<img width="940" height="547" alt="image" src="https://github.com/user-attachments/assets/38e1304f-3d99-4393-9911-33fb75627cfd" />
Backend:
<img width="940" height="499" alt="image" src="https://github.com/user-attachments/assets/b8c39caa-855a-4114-ab7c-5350de84d2c8" />
<img width="940" height="442" alt="image" src="https://github.com/user-attachments/assets/65714a56-b806-488f-8b2e-d95ec5a1d248" />
<img width="1012" height="741" alt="image" src="https://github.com/user-attachments/assets/ef400dfb-62c4-48f7-aa9f-9869bdff9a93" />














