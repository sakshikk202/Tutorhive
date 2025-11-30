# TutorHive - AI-Powered Tutoring Platform

A modern, responsive tutoring platform that connects students with expert tutors through an AI-enhanced learning experience. Built with Next.js 14, React 18, Tailwind CSS, and developed with AI assistance using GPT-5 model.

## Project Overview

TutorHive is a comprehensive tutoring platform designed to facilitate personalized learning experiences between students and qualified tutors. The platform leverages AI technology to provide intelligent study recommendations, progress tracking, and enhanced learning outcomes.

This document outlines the comprehensive development contributions made during Phase 1
(Planning), Phase 2 (Frontend), and Phase 3 (Backend & Integration) of the TutorHive project.
The team has successfully delivered a fully integrated, production-ready full-stack application.

## Scope

Phase Focus: Full Stack Development (Frontend + Backend + AI) Duration: Phases 1, 2, & 3
Technology Stack:
- **Frontend**: Next.js 14, React 18, Tailwind CSS 4, Radix UI
- **Backend**: Node.js, Express, Supabase Edge Functions
- **Database**: Supabase (PostgreSQL), Supabase Storage
- **AI**: Groq API (Llama 3.3 70b Model)

## Project deploy at : https://tutor-hive-new.vercel.app/

## Team Members

- **Gunturu, Ainesh** (1002248191) - Team Lead
- **Garikipati, Jahnavi** (1002200930) - Frontend + AI Researcher
- **Jawahar, Narain Sarathy** (1002223825) - Documentation + Tester
- **Katakam, Amruth Bhargav** (1002237703) - UX Designer
- **Khanapure, Sakshi Omprakash** (1002175905) - Scrum Reporter + Backend

## UTA Cloud Deployment:

    URL - https://axg8191.uta.cloud/
    Credentials - 
        student login
        email :- student@example.com
        password:- student123
        tutor login
        email:- tutor@example.com
        password:- tutor123

## Github Repo 
https://github.com/sakshikk202/Tutorhive

## Key Features

### For Students
- **Expert Tutor Matching**: Connect with qualified tutors specializing in various subjects
- **Flexible Scheduling**: Book sessions that fit your schedule with an intuitive calendar system
- **AI Study Assistant**: Get personalized study recommendations and progress tracking
- **Study Plans**: Create and follow AI-generated study plans tailored to your learning goals
- **Session Management**: Track upcoming and past tutoring sessions
- **Progress Tracking**: Monitor your learning progress with detailed analytics
- **Task Management**: Create and manage study tasks and assignments

### For Tutors
- **Tutor Registration**: Easy onboarding process with subject specialization
- **Student Management**: View and manage your students and sessions
- **Session Scheduling**: Set your availability and manage bookings
- **Performance Analytics**: Track your teaching performance and student outcomes
- **Profile Management**: Maintain your professional profile and credentials

### Platform Features
- **AI-Enhanced Learning**: Intelligent recommendations and personalized content
- **Responsive Design**: Works seamlessly across desktop, tablet, and mobile devices
- **Dark/Light Mode**: User preference-based theme switching
- **Real-time Chat**: Integrated communication system for students and tutors
- **Secure Authentication**: Role-based access control for students and tutors
- **Modern UI/UX**: Clean, intuitive interface built with modern design principles

## Technology Stack

### Frontend
- **React 18** - UI library
- **Tailwind CSS 4.1.9** - Utility-first CSS framework
- **Radix UI** - Accessible component primitives
- **Lucide React** - Icon library
- **Recharts** - Data visualization
- **React Hook Form** - Form management
- **Zod** - Schema validation
- **GPT-5 Model** - AI-assisted code generation and optimization

### Backend & Database
- **Platform**: Supabase (BaaS)
- **Database**: PostgreSQL
- **Security**: RLS (Row Level Security) Policies
- **Compute**: Supabase Edge Functions (Deno/Node.js)
- **Storage**: Supabase Storage Buckets

### AI Stack
- **Provider**: Groq Cloud API
- **Model**: Llama 3.3 70b Versatile
- **Integration**: Server-side calls via Edge Functions to protect API keys


### Styling & Design
- **Custom CSS Variables** - Theme system with light/dark mode support
- **Fonts**: Source Sans 3 (primary), Playfair Display (headings), Geist Mono (code)
- **Color Palette**: 
  - Primary: Dark teal (#164e63)
  - Secondary: Indigo (#6366f1)
  - Accent: Orange (#d97706)
  - Background: White/Dark variants
  - Destructive: Red (#ef4444)

### Development Tools
- **TypeScript** - Type safety
- **ESLint** - Code linting
- **PostCSS** - CSS processing
- **Autoprefixer** - CSS vendor prefixing
- **GPT-5 Model** - AI-assisted development and code optimization

### AI-Assisted Development Areas
- **Project Scaffolding**: AI-generated project structure and configuration
- **Component Generation**: AI-assisted creation of 50+ reusable UI components
- **Styling Implementation**: AI-powered Tailwind CSS class generation and responsive design
- **Testing Framework**: AI-generated test cases and component testing strategies
- **Code Optimization**: AI-assisted performance optimization and best practices implementation


## Project Structure

```
tutoring-platform/
├── app/                         
│   ├── ai-assistant/            # AI study assistant (AI-assisted)
│   │   └── page.jsx             # AI chat interface and tools
│   ├── connections/             # Student-tutor connections
│   ├── dashboard/               # Main dashboard (student & tutor) (AI-assisted)
│   │   ├── page.jsx             # Student dashboard with stats and quick actions
│   │   └── tutor/               # Tutor-specific dashboard
│   ├── login/                   # Authentication pages (AI-assisted)
│   │   └── page.jsx             # Login form with role selection
│   ├── register/                # User registration (AI-assisted)
│   │   └── page.jsx             # Registration form with validation
│   ├── sessions/                # Session management (AI-assisted)
│   │   ├── book/               # Session booking
│   │   ├── calendar/           # Calendar view
│   │   ├── [id]/               # Individual session pages
│   │   └── page.jsx             # Sessions overview and management
│   ├── study-plans/            # Study plan management (AI-assisted)
│   │   ├── create/             # Create study plans
│   │   ├── [id]/               # Individual study plans
│   │   └── page.jsx             # Study plans overview
│   ├── tasks/                  # Task management (AI-assisted)
│   │   ├── create/             # Task creation
│   │   └── page.jsx             # Task management interface
│   ├── tutors/                 # Tutor discovery and ranking
│   ├── tutor-registration/     # Tutor onboarding (AI-assisted)
│   │   └── page.jsx             # Tutor registration form
│   ├── profile/                # User profiles
│   ├── settings/               # User settings
│   ├── inbox/                  # Messaging system
│   ├── globals.css             # Global styles and theme (AI-assisted design system)
│   ├── layout.jsx              # Root layout (AI-assisted)
│   └── page.jsx                # Landing page (AI-assisted)
├── components/                  # Reusable UI components
│   ├── ui/                     # Base UI components (Radix UI) (AI-assisted)
│   │   ├── button.jsx          # Button component with variants
│   │   ├── card.jsx            # Card component with sections
│   │   ├── input.jsx           # Input component with validation
│   │   ├── form.jsx            # Form component with React Hook Form
│   │   ├── select.jsx          # Select dropdown component
│   │   ├── calendar.jsx        # Calendar component for scheduling
│   │   └── ...                 # 50+ other UI components
│   ├── ai-chat-widget.jsx      # AI chat interface (AI-assisted)
│   ├── ai-recommendations.jsx  # AI study recommendations (AI-assisted)
│   ├── dashboard-nav.jsx       # Navigation component (AI-assisted)
│   └── task-item.jsx           # Task display component
├── hooks/                      # Custom React hooks
├── lib/                        # Utility functions
├── public/                     # Static assets
├── styles/                     # Additional stylesheets
├── next.config.mjs             # Next.js configuration (AI-assisted)
├── package.json                # Dependencies and scripts (AI-assisted)
└── README.md                   # Project documentation
```
## Available Pages & Routes

### Public Pages
- `/` - Landing page with features and hero section
- `/login` - User authentication (Student/Tutor)
- `/register` - User registration
- `/forgot-password` - Password recovery

### Student Dashboard
- `/dashboard` - Main student dashboard
- `/sessions` - View all sessions
- `/sessions/book` - Book new sessions
- `/sessions/calendar` - Calendar view
- `/sessions/[id]` - Individual session details
- `/study-plans` - View study plans
- `/study-plans/create` - Create new study plan
- `/study-plans/[id]` - Individual study plan
- `/tasks` - Task management
- `/tasks/create` - Create new task
- `/tutors/ranking` - Browse and find tutors
- `/ai-assistant` - AI study assistant
- `/profile` - User profile
- `/settings` - Account settings
- `/inbox` - Messaging system
- `/connections` - Student-tutor connections

### Tutor Dashboard
- `/dashboard/tutor` - Tutor-specific dashboard
- `/tutor-registration` - Tutor onboarding process

## Design System

### Typography
- **Primary Font**: Source Sans 3 (sans-serif)
- **Heading Font**: Playfair Display (serif)
- **Code Font**: Geist Mono (monospace)

### Color Scheme
- **Primary**: Dark teal (#164e63) - Main brand color
- **Secondary**: Indigo (#6366f1) - Accent color
- **Accent**: Orange (#d97706) - Highlight color
- **Background**: White (#ffffff) / Dark (#252525)
- **Foreground**: Slate gray (#475569) / White
- **Destructive**: Red (#ef4444) - Error states

### Components
Built with Radix UI primitives for accessibility and consistency:

#### Core Re-usable React UI Components (`@/components/ui/`)
- **Button** - Multiple variants (default, destructive, outline, secondary, ghost, link)
- **Card** - Container with header, content, and footer sections
- **Input** - Form input with validation states and focus styles
- **Label** - Accessible form labels
- **Textarea** - Multi-line text input
- **Select** - Dropdown selection with search and grouping
- **Checkbox** - Custom checkbox with indeterminate state
- **Radio Group** - Radio button groups with keyboard navigation
- **Switch** - Toggle switch component
- **Slider** - Range input slider
- **Progress** - Progress bar with animated states
- **Badge** - Status indicators and labels
- **Avatar** - User profile images with fallbacks
- **Separator** - Visual dividers (horizontal/vertical)

#### Layout & Navigation
- **Sidebar** - Collapsible navigation sidebar
- **Navigation Menu** - Multi-level navigation with dropdowns
- **Breadcrumb** - Navigation breadcrumbs
- **Tabs** - Tabbed content organization
- **Accordion** - Collapsible content sections
- **Collapsible** - Simple collapsible content
- **Menubar** - Horizontal menu bar
- **Command** - Command palette with search
- **Scroll Area** - Custom scrollable areas

#### Overlays & Modals
- **Dialog** - Modal dialogs with backdrop
- **Alert Dialog** - Confirmation and alert modals
- **Sheet** - Slide-out panels (bottom, left, right, top)
- **Drawer** - Mobile-friendly slide-out drawer
- **Popover** - Floating content containers
- **Tooltip** - Contextual information tooltips
- **Hover Card** - Rich hover content cards
- **Context Menu** - Right-click context menus
- **Dropdown Menu** - Dropdown menus with icons and separators

#### Data Display
- **Table** - Data tables with sorting and selection
- **Chart** - Data visualization components (Recharts integration)
- **Calendar** - Date picker and calendar views
- **Carousel** - Image/content carousels
- **Aspect Ratio** - Maintain aspect ratios for media
- **Skeleton** - Loading state placeholders

#### Forms & Input
- **Form** - React Hook Form integration with validation
- **Input OTP** - One-time password input
- **Toggle** - Toggle buttons and groups
- **Toggle Group** - Grouped toggle buttons

#### Feedback & Notifications
- **Alert** - Alert messages with variants
- **Toast** - Toast notifications with actions
- **Toaster** - Toast container and management
- **Sonner** - Advanced toast notifications

#### Utilities
- **Resizable** - Resizable panels and containers
- **Pagination** - Page navigation controls
- **Use Mobile** - Mobile detection hook
- **Use Toast** - Toast management hook

#### Design Features
- Responsive design with mobile-first approach
- Dark/light mode support with CSS variables
- Accessibility compliance (WCAG 2.1)
- Keyboard navigation support
- Focus management and screen reader support
- Consistent spacing and typography
- Customizable theming system

## Configuration

### Configuration
- **Output**: Static export for deployment
- **Image Optimization**: Disabled for static export
- **TypeScript**: Enabled with build error tolerance
- **ESLint**: Configured with build error tolerance

### Tailwind CSS
- Custom color variables for theming
- Responsive breakpoints
- Custom animations and transitions
- Component-based styling approach

## Features in Detail

### AI Integration
- **Study Recommendations**: AI-powered personalized study suggestions
- **Progress Analysis**: Intelligent tracking of learning progress
- **Chat Assistant**: Real-time AI assistance for students
- **Smart Matching**: Algorithm-based tutor-student matching

### Session Management
- **Calendar Integration**: Visual scheduling interface
- **Booking System**: Easy session booking process
- **Session History**: Complete record of past sessions
- **Real-time Updates**: Live session status updates

### Study Planning
- **Custom Plans**: Create personalized study schedules
- **Goal Setting**: Define and track learning objectives
- **Progress Tracking**: Monitor completion and performance
- **AI Suggestions**: Intelligent plan recommendations

## Major Achievements

### 1. **Architecture**
- **react 18 App Router**: Implemented modern routing with App Router
- **Next.js 14 App Router**: Modern routing for optimal performance
- **Component-Based Architecture**: Built modular, reusable component system
- **TypeScript Integration**: Added type safety throughout the application
- **Responsive Design**: Mobile-first approach with full responsiveness

### 2. **Comprehensive UI Component Library**
- **50+ Reusable Components**: Built complete component library using Radix UI
- **Accessibility Compliance**: WCAG 2.1 compliant components
- **Theme System**: Custom CSS variables for consistent theming
- **Dark/Light Mode**: Complete theme switching functionality

### 3. **User Interface Pages (20+ Pages)**
- **Landing Page**: Modern hero section with features showcase
- **Authentication**: Login/Register with role-based access (Student/Tutor). Secure Email/Password and OAuth flows via Supabase Auth.
- **Student Dashboard**: Comprehensive student interface with quick actions
- **Tutor Dashboard**: Specialized tutor interface and management. Visual progress tracking and session history.
- **Session Management**: Booking, calendar, and session tracking
- **Study Plans**: Create, view, and manage personalized study plans
- **Task Management**: Task creation, tracking, and completion
- **AI Assistant**: Interactive AI chat and recommendations
- **Tutor Discovery**: Browse and find tutors with ranking system. Advanced filtering and full-text search for tutors.
- **Profile Management**: User profiles and settings
- **Messaging System**: Inbox and communication interface

### 4. **Advanced Features Implementation**
- **AI Chat Widget**: Floating AI assistant with real-time chat
- **AI Recommendations**: Intelligent study recommendations system
- **Calendar Integration**: Session booking and scheduling interface
- **Progress Tracking**: Visual progress indicators and analytics
- **Real-time Updates**: Dynamic content updates and notifications
- **Form Validation**: Comprehensive form validation with error handling

### 5. **AI-Assisted Development Achievements**
- **Rapid Development**: 50+ components built with AI assistance in record time
- **Consistent Styling**: AI-generated Tailwind CSS ensuring design consistency
- **Quality Code**: AI-assisted code generation following best practices
- **Comprehensive Testing**: AI-generated test strategies covering all aspects
- **Performance Optimization**: AI-powered bundle optimization and performance tuning
- **Accessibility Compliance**: AI-assisted WCAG 2.1 compliance implementation
- **Groq & Llama 3.3**: High-performance AI integration using the Llama 3.3 70b model via
Groq.
- **Contextual Chat**: AI assistant maintains conversation context for tutoring help.
- **Smart Recommendations**: Algorithm matching students with tutors based on subject
and availability.

### 6. Robust Backend Infrastructure
- **Supabase Integration**: Fully managed PostgreSQL database with Row Level Security
(RLS).
- **Edge Functions**: Serverless functions handling secure operations and AI requests.
- **Real-time Capabilities**: WebSocket connections for instant chat and status updates
- **Secure Storage**: Scalable file storage for user generated content.

---

### **Key Components Developed**

#### **Core UI Components**
- Button (6 variants), Card, Input, Label, Textarea
- Select, Checkbox, Radio Group, Switch, Slider
- Progress, Badge, Avatar, Separator
- Form components with validation

#### **Layout Components**
- Sidebar, Navigation Menu, Breadcrumb
- Tabs, Accordion, Collapsible
- Command palette, Scroll areas

#### **Overlay Components**
- Dialog, Alert Dialog, Sheet, Drawer
- Popover, Tooltip, Hover Card
- Context Menu, Dropdown Menu

#### **Data Display**
- Table with sorting and selection
- Chart components for analytics
- Calendar for scheduling
- Carousel for content display

#### **Custom Components**
- `DashboardNav` - Responsive navigation system
- `AIChatWidget` - Floating AI assistant
- `AIRecommendations` - Smart study suggestions
- `TaskItem` - Task management component

### **Design System Implementation**
- **Color Palette**: Primary (Dark Teal), Secondary (Indigo), Accent (Orange)
- **Typography**: Source Sans 3, Playfair Display, Geist Mono
- **Spacing**: Consistent spacing system with Tailwind
- **Shadows**: Layered shadow system for depth
- **Animations**: Smooth transitions and micro-interactions

---

## Responsive Design Implementation

### **Breakpoints**
- **Mobile**: 320px - 768px (Mobile-first approach)
- **Tablet**: 768px - 1024px
- **Desktop**: 1024px+ (Large screens)

### **Mobile Features**
- **Touch-friendly**: Large touch targets and gestures
- **Mobile Navigation**: Hamburger menu and mobile-optimized navigation
- **Responsive Grid**: Adaptive grid layouts for all screen sizes
- **Mobile Forms**: Optimized form layouts for mobile input

---

## User Experience Features

### **Student Experience**
- **Intuitive Dashboard**: Quick access to all features
- **Easy Session Booking**: Simple calendar-based booking
- **AI-Powered Learning**: Smart recommendations and assistance
- **Progress Tracking**: Visual progress indicators
- **Study Plan Management**: Create and follow personalized plans

### **Tutor Experience**
- **Professional Dashboard**: Tutor-specific interface
- **Student Management**: View and manage students
- **Session Scheduling**: Set availability and manage bookings
- **Performance Analytics**: Track teaching performance

### **Accessibility Features**
- **Keyboard Navigation**: Full keyboard accessibility
- **Screen Reader Support**: ARIA labels and semantic HTML
- **High Contrast**: Support for high contrast modes
- **Focus Management**: Clear focus indicators
- **Color Blindness**: Color-blind friendly design

---

## Development Process

### **Development Methodology**
- **Agile Development**: Sprint-based development with regular reviews
- **Component-First**: Built reusable components before pages
- **Mobile-First**: Responsive design starting from mobile
- **Accessibility-First**: Built with accessibility in mind
- **AI-Assisted Development**: Leveraged GPT-5 model for efficient code generation and optimization

### **AI-Assisted Development Process**
- **GPT-5 Integration**: Utilized GPT-5 model for intelligent code generation and optimization
- **Code Generation**: AI-assisted creation of complex components and functionality
- **Code Optimization**: AI-powered code refactoring and performance improvements
- **Best Practices**: AI guidance for following React and Next.js best practices
- **Rapid Prototyping**: Accelerated development through AI-assisted component creation
- **Quality Assurance**: AI-assisted code review and bug detection

### **Specific AI Implementation Areas**

#### **Project Scaffolding**
- **Next.js 14 Setup**: AI-generated project structure with App Router configuration
- **Package.json Configuration**: AI-assisted dependency management and script setup
- **TypeScript Configuration**: AI-generated tsconfig.json and type definitions
- **Tailwind CSS Setup**: AI-configured Tailwind CSS with custom design system
- **Component Library Structure**: AI-designed folder structure for UI components
- **Routing Architecture**: AI-planned page routing and navigation structure

#### **Styling and Design System**
- **CSS Variables**: AI-generated custom CSS variables for theming system
- **Color Palette**: AI-assisted color scheme selection and implementation
- **Typography System**: AI-generated font configurations and text styling
- **Responsive Design**: AI-powered responsive breakpoints and mobile-first approach
- **Component Styling**: AI-generated Tailwind CSS classes for all UI components
- **Dark/Light Mode**: AI-implemented theme switching functionality
- **Animation System**: AI-generated CSS animations and transitions

#### **Testing and Quality Assurance**
- **Component Testing**: AI-generated test cases for UI component functionality
- **Cross-browser Testing**: AI-assisted testing strategies for browser compatibility
- **Accessibility Testing**: AI-generated accessibility test cases and WCAG compliance checks
- **Performance Testing**: AI-assisted performance optimization and bundle analysis
- **User Experience Testing**: AI-generated usability testing scenarios
- **Code Quality Checks**: AI-assisted ESLint configuration and code formatting

### **Code Quality**
- **TypeScript**: Type safety throughout the application
- **ESLint**: Code linting and formatting
- **Component Documentation**: Comprehensive component docs
- **Code Reviews**: Regular peer code reviews

### **Testing Approach**
- **Cross-browser Testing**: Chrome, Firefox, Safari, Edge
- **Device Testing**: Mobile, tablet, desktop devices
- **Accessibility Testing**: Screen reader and keyboard testing
- **User Testing**: Usability testing with target users

---

## Performance Optimizations

### **Frontend Performance**
- **Code Splitting**: Automatic code splitting with react
- **Image Optimization**: Optimized images and lazy loading
- **Bundle Size**: Minimized JavaScript bundle size
- **Caching**: Efficient caching strategies
- **Loading States**: Skeleton screens and loading indicators

### **User Experience Optimizations**
- **Fast Loading**: Optimized for quick page loads
- **Smooth Animations**: 60fps animations and transitions
- **Responsive Images**: Adaptive images for different screen sizes
- **Progressive Enhancement**: Works without JavaScript

---

## Deployment Preparation

### **Static Export Configuration**
- **react Static Export**: Configured for static site generation
- **Image Optimization**: Unoptimized images for static export
- **Build Optimization**: Optimized build process
- **Deployment Ready**: Ready for Vercel, Netlify, or any static hosting

---

## Project Metrics

### **Code Statistics**
- **Total Files**: 100+ files
- **Components**: 50+ reusable UI components
- **Pages**: 20+ application pages
- **Lines of Code**: 10,000+ lines of frontend code
- **Bundle Size**: Optimized for production

### **Features Implemented**
- **Authentication System**: Complete login/register flow
- **Dashboard Systems**: Student and tutor dashboards
- **Session Management**: Full session lifecycle
- **AI Integration**: Chat and recommendations
- **Study Planning**: Complete study plan system
- **Task Management**: Full task lifecycle
- **Profile Management**: User profiles and settings

---

## Backend Integration

### **API Integration Points**
- **Authentication APIs**: Login, register, password reset
- **User Management**: Profile CRUD operations
- **Session APIs**: Booking, scheduling, management
- **AI Integration**: Backend AI service integration
- **Real-time Features**: WebSocket integration for chat
- **File Upload**: Profile images and document uploads

### **Data Flow Preparation**
- **State Management**: Redux/Zustand for global state
- **API Client**: Axios/Fetch wrapper for API calls
- **Error Handling**: Comprehensive error handling system
- **Loading States**: Loading indicators for async operations
---

## Deployment

The project is configured for static export and can be deployed to:
- Vercel
- Netlify
- GitHub Pages
- Any static hosting service

Build command: `npm run build`
Output directory: `out/`

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request


## Team Contributions

### **Gunturu, Ainesh** (1002248191) - Team Lead
**Role**: Project Management, Architecture and Security
- **Project Architecture**: Designed the end-to-end architecture connecting Next.js frontend with Supabase backend.
- **Technology Stack Selection**: Chose react 14 with App Router for optimal performance
- **Component Library Setup**: Implemented comprehensive UI component library with Radix UI
- **Code Quality**: Established coding standards and best practices
- **Integration**: Coordinated frontend-backend integration planning
- **Documentation**: Created comprehensive project documentation and README
- **Security Protocols**: Implemented RLS (Row Level Security) policies and secured API
keys using Edge Functions
- **Search Logic**: Designed and optimized PostgreSQL Full Text Search algorithms for the
"Find a Tutor" feature.
- **Deployment**: Managed the CI/CD pipelines and final production deployment of both
frontend and backend.
- **Performance**: Optimized database indexing and API response times.


### **Garikipati, Jahnavi** (1002200930) - Frontend + AI Researcher
**Role**: Core Frontend Development, AI Integration and interactive features
- **AI Assistant Implementation**: Connected the frontend Chat Widget to Groq AI using Llama 3.3
70b
- **Dashboard Development**: Created student and tutor dashboard layouts
- **AI Recommendations**: Implemented AI-powered study recommendations system
- **Interactive Components**: Developed dynamic UI components with real-time features
- **State Management**: Implemented React state management for complex interactions
- **AI Integration**: Designed AI-powered features and chat interfaces
- **User Experience**: Focused on intuitive AI interactions and recommendations
- **AI-Assisted Scaffolding**: Used GPT-5 for rapid component generation and project structure
- **AI-Powered Styling**: Leveraged AI for Tailwind CSS class generation and responsive design
- **AI Testing Strategies**: Implemented AI-generated testing approaches for component validation
- **Real-time Features**: Implemented Supabase Realtime for live chat and session updates.
- **Prompt Engineering**: Refined system prompts for the Llama 3.3 model to ensure
academic relevance.
- **Frontend-Backend Bridge**: Integrated all frontend forms (Login, Profile, Booking) with
backend APIs.


### **Jawahar, Narain Sarathy** (1002223825) - Documentation + Tester
**Role**: Quality Assurance & Documentation
- **Component Testing**: Tested all UI components for functionality and responsiveness
- **Cross-browser Testing**: Ensured compatibility across different browsers
- **Code Review**: Performed thorough code reviews for quality assurance
- **User Testing**: Conducted usability testing and feedback collection
- **Bug Reporting**: Identified and documented issues for resolution
- **Accessibility Testing**: Ensured WCAG compliance and accessibility standards
- **AI-Generated Test Cases**: Utilized GPT-5 for comprehensive test case generation
- **AI-Assisted Testing Strategies**: Implemented AI-recommended testing methodologies
- **AI Documentation**: Used AI assistance for technical documentation and guides
- **API Testing**: Conducted comprehensive testing of all Supabase endpoints and RLS
policies.
- **E2E Testing**: Performed full End-to-End user journey tests (SignUp -> Search -> Book ->
Chat).
- **Documentation**: - Created detailed component documentation, usage guides and Swagger/OpenAPI documentation for backend APIs and
Supabase tables.
- **Load Testing**: Tested search query performance and session booking concurrency.
- **Bug Reporting**: Managed the issue tracker for integration bugs.


### **Katakam, Amruth Bhargav** (1002237703) - UX Designer
**Role**: User Experience & Visual Design
- **UI/UX Design**: Created complete visual design system and user interface
- **Design System**: Established color palette, typography, and component guidelines.Designed Empty, Loading, and Error states for all data-driven components.
- **User Journey Mapping**: Designed user flows for students and tutors
- **Responsive Design**: Ensured mobile-first responsive design across all devices
- **Visual Components**: Designed custom icons, layouts, and visual elements
- **Theme System**: Implemented dark/light mode theming system
- **Accessibility Design**: Ensured inclusive design principles and accessibility
- **AI-Enhanced Design System**: Used GPT-5 for color palette optimization and typography selection
- **AI-Generated CSS**: Leveraged AI for complex CSS animations and responsive breakpoints
- **AI Design Patterns**: Implemented AI-recommended design patterns and user experience flows
- **Admin/Feedback UI**: Designed toast notifications and feedback loops for API actions.
- **Chat UX**: Polished the visual interface of the AI chat bubbles and typing indicators.
- **Responsive Audit**: Ensured complex tables (Calendars, Schedules) remained
responsive with real data.

### **Khanapure, Sakshi Omprakash** (1002175905) - Scrum Reporter + Backend
**Role**: Project Coordination & Backend Integration
- **Database Schema**: Designed and implemented the normalized PostgreSQL schema
(Users, Profiles, Sessions, Bookings).
- **Sprint Management**: Coordinated development sprints and task distribution
- **Progress Tracking**: Monitored development progress and milestone completion
- **Backend Integration**: Prepared frontend for backend API integration
- **Backend Logic**: Developed Supabase Edge Functions for complex business logic (e.g.,
matching).
- **Data Flow Design**: Designed data flow between frontend and backend systems
- **API Implementation**: Built CRUD endpoints for Sessions, Tasks, and Profiles.
- **Performance Optimization**: Focused on frontend performance and optimization
- **AI Project Management**: Used GPT-5 for sprint planning and task breakdown
- **AI Performance Analysis**: Leveraged AI for frontend performance optimization strategies
- **AI Integration Planning**: Utilized AI assistance for API integration architecture design
- **Storage Configuration**: Configured Supabase Storage buckets for secure user avatar
and document uploads.

## Team Achievements

### **Collective Accomplishments**
- **Complete Frontend Architecture** - Built from scratch
- **50+ Reusable Components** - Comprehensive UI library
- **20+ Application Pages** - Full user journey coverage
- **Mobile-First Design** - Responsive across all devices
- **Accessibility Compliance** - WCAG 2.1 standards
- **AI Integration Ready** - Frontend prepared for AI services
- **Production Ready** - Optimized for deployment
- **Documentation Complete** - Comprehensive documentation

### **Individual Contributions Summary**
- **Gunturu, Ainesh**: System Architecture, Security, Search Algorithms, and Deployment.
- **Garikipati, Jahnavi**: AI Service Integration, Real-time Chat, and Frontend Logic.
- **Jawahar, Narain Sarathy**: E2E Testing, API Validation, and Technical Documentation.
- **Katakam, Amruth Bhargav**: UI/UX for Data States, Visual Polish, and User Guides.
- **Khanapure, Sakshi Omprakash**: Database Schema Design, Backend API Development, and Project
Management.
---

# Setup Guide - Tutoring Platform

This guide will help you set up and run the Tutoring Platform project on your local machine.

## Prerequisites

Before you begin, make sure you have the following installed:

- **Node.js** (version 18 or higher) - [Download](https://nodejs.org/)
- **PostgreSQL** (version 12 or higher) - [Download](https://www.postgresql.org/download/)
- **npm** or **pnpm** (comes with Node.js, or install pnpm separately)
- **Git** (optional, for cloning the repository)

## Step 1: Clone/Download the Project

If you received this project via Git:
```bash
git clone <repository-url>
cd tutoring-platform
```

If you received it as a zip file, extract it and navigate to the project directory:
```bash
cd tutoring-platform
```

## Step 2: Install Dependencies

Install all project dependencies using npm or pnpm:

```bash
# Using npm
npm install

# OR using pnpm (if you have it installed)
pnpm install
```

This will install all required packages listed in `package.json`.

## Step 3: Set Up PostgreSQL Database

1. **Create a PostgreSQL database:**
   ```bash
   # Login to PostgreSQL (you may need to enter your PostgreSQL password)
   psql -U postgres
   
   # Create a new database
   CREATE DATABASE tutoring_platform;
   
   # Exit PostgreSQL
   \q
   ```

   **Note:** If you're on macOS and installed PostgreSQL via Homebrew, you might need to use:
   ```bash
   psql postgres
   ```

2. **Alternative:** You can also use a cloud PostgreSQL service like:
   - [Supabase](https://supabase.com/) (free tier available)
   - [Railway](https://railway.app/) (free tier available)
   - [Neon](https://neon.tech/) (free tier available)
   - [ElephantSQL](https://www.elephantsql.com/) (free tier available)

## Step 4: Configure Environment Variables

Create a `.env` file in the root directory of the project:

```bash
touch .env
```

Open the `.env` file and add the following environment variables:

```env
# Database Configuration (REQUIRED)
DATABASE_URL="postgresql://username:password@localhost:5432/tutoring_platform?schema=public"

# Replace with your actual PostgreSQL credentials:
# - username: your PostgreSQL username (default: postgres)
# - password: your PostgreSQL password
# - localhost: your database host (use your cloud provider's URL if using cloud PostgreSQL)
# - 5432: PostgreSQL port (default is 5432)
# - tutoring_platform: the database name you created

# Example for local PostgreSQL:
# DATABASE_URL="postgresql://postgres:yourpassword@localhost:5432/tutoring_platform?schema=public"

# Example for cloud PostgreSQL (Supabase/Railway/etc):
# DATABASE_URL="postgresql://user:password@host.region.provider.com:5432/tutoring_platform?schema=public"

# AI Chat Configuration (REQUIRED for AI features)
GROQ_API_KEY="your_groq_api_key_here"

# Get your Groq API key from: https://console.groq.com/
# Sign up for a free account and generate an API key
# The AI chat widget will not work without this key

# Optional: Specify Groq model (defaults to llama-3.3-70b-versatile if not set)
GROQ_MODEL="llama-3.3-70b-versatile"

# Optional: Server Configuration
PORT=3000

# Optional: Notification Reminders Secret Key (for scheduled reminders)
REMINDER_SECRET_KEY="your-secret-key-here"

# Optional: Node Environment
NODE_ENV="development"
```

### Getting Your Groq API Key

1. Visit [Groq Console](https://console.groq.com/)
2. Sign up for a free account (if you don't have one)
3. Navigate to API Keys section
4. Create a new API key
5. Copy the key and paste it in your `.env` file as `GROQ_API_KEY`

**Important:** Never commit your `.env` file to version control! It's already in `.gitignore`.

## Step 5: Run Database Migrations

After setting up your database and environment variables, run Prisma migrations to create the database schema:

```bash
# Generate Prisma Client
npx prisma generate

# Run database migrations
npx prisma migrate dev

# This will:
# - Create all database tables based on the schema
# - Set up relationships between tables
# - Create indexes for better performance
```

## Step 6: Seed the Database (Optional but Recommended)

Seed the database with sample data to test the application:

```bash
npm run seed
```

This will create:
- Sample users (both students and tutors)
- Sample tutor profiles with subjects and ratings
- All users can login with password: `password123`

**Sample User Emails (all use password: `password123`):**
- `michael.chen@university.edu`
- `emily.rodriguez@university.edu`
- `david.kim@university.edu`
- `sarah.johnson@university.edu`

## Step 7: Start the Development Server

Start the Next.js development server:

```bash
npm run dev
```

The application will start at `http://localhost:3000` (or the port you specified in `.env`).

You should see output like:
```
> Ready on http://localhost:3000
```

## Step 8: Access the Application

Open your web browser and navigate to:
```
http://localhost:3000
```

You should see the tutoring platform homepage!

## Troubleshooting

### Database Connection Issues

**Problem:** "Can't reach database server" or connection errors

**Solutions:**
1. Verify PostgreSQL is running:
   ```bash
   # macOS
   brew services list
   
   # Linux
   sudo systemctl status postgresql
   
   # Windows
   # Check Services panel
   ```

2. Double-check your `DATABASE_URL` in `.env`:
   - Verify username and password are correct
   - Ensure database name exists
   - Check host and port are correct

3. Test database connection:
   ```bash
   psql $DATABASE_URL
   ```

### Prisma Client Issues

**Problem:** "Prisma Client has not been initialized" or model errors

**Solution:**
```bash
npx prisma generate
```

### Port Already in Use

**Problem:** "Port 3000 is already in use"

**Solutions:**
1. Use a different port in `.env`:
   ```env
   PORT=3001
   ```

2. Or kill the process using port 3000:
   ```bash
   # macOS/Linux
   lsof -ti:3000 | xargs kill -9
   ```

### AI Chat Not Working

**Problem:** AI chat widget shows errors or doesn't respond

**Solutions:**
1. Verify `GROQ_API_KEY` is set in `.env`
2. Check that the API key is valid at [Groq Console](https://console.groq.com/)
3. Restart the development server after adding the key:
   ```bash
   # Stop the server (Ctrl+C) and restart
   npm run dev
   ```

### Module Not Found Errors

**Problem:** "Cannot find module" errors

**Solution:**
```bash
# Delete node_modules and reinstall
rm -rf node_modules package-lock.json
npm install
```

## Project Structure

- `/app` - Next.js app directory with pages and API routes
- `/components` - React components and UI elements
- `/lib` - Utility functions and database client
- `/prisma` - Database schema and migrations
- `/public` - Static assets (images, etc.)
- `/hooks` - Custom React hooks

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run seed` - Seed database with sample data
- `npx prisma studio` - Open Prisma Studio to view/edit database (optional)

## Production Deployment

For production deployment:

1. Set `NODE_ENV=production` in your production environment
2. Use a production-ready PostgreSQL database
3. Build the application:
   ```bash
   npm run build
   ```
4. Start the production server:
   ```bash
   npm run start
   ```

## Additional Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [Prisma Documentation](https://www.prisma.io/docs)
- [Groq API Documentation](https://console.groq.com/docs)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)

## In case of error

If you encounter any issues:
1. Check the Troubleshooting section above
2. Verify all environment variables are set correctly
3. Ensure all dependencies are installed
4. Check that PostgreSQL is running and accessible
5. Review the console/terminal for error messages

## Conclusion

The TutorHive project has successfully delivered a complete, production-ready full-stack application. The team has built a modern, accessible, and intelligent tutoring platform that leverages the latest technologies in AI (Groq/Llama 3.3) and Backend-as-a-Service (Supabase).

The platform is fully functional, featuring secure authentication, real-time AI assistance, and robust session management. All project phases (Planning, Frontend, Backend) have been completed on schedule with high quality.

Total Development Time: Phases 1, 2 & 3 (Full Stack Complete) - 12 weeks
Status: Complete and Deployed 
Final Outcome: A scalable, AI-powered educational platform ready for users.

This document represents the comprehensive full-stack development contributions made by the TutorHive development team throughout the project lifecycle.

## License

This project is part of an academic assignment and is not intended for commercial use.

