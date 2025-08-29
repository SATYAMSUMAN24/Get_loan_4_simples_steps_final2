# Overview

This is a comprehensive digital loan processing platform that provides a complete 4-step loan application system. The application guides users through loan selection, personal information collection, income details, and offer presentation. It features dynamic EMI calculations, form validation, mobile verification, and document upload capabilities. The system supports multiple loan types (Home, Personal, Vehicle, Education) with conditional sub-categories and employment type selections.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Technology Stack**: Pure HTML5, CSS3, and vanilla JavaScript
- **Design Pattern**: Single Page Application (SPA) with step-based navigation
- **State Management**: Global JavaScript object (`formData`) for maintaining application state
- **UI Components**: Modular step-based interface with progress stepper, form validation, and dynamic content display
- **Responsive Design**: Mobile-first approach with flexible layouts

## Form Management System
- **Multi-Step Flow**: 4-step wizard interface (Basic Details → Personal Details → Income Details → Your Offer)
- **Data Persistence**: Local storage implementation for saving user progress
- **Validation Engine**: Real-time form validation with visual feedback
- **Dynamic Forms**: Conditional field display based on loan type selection (e.g., vehicle sub-types)

## Calculation Engine
- **EMI Calculator**: Real-time EMI calculation based on loan amount, interest rate, and tenure
- **Auto-calculation**: Dynamic updates when users modify loan parameters
- **Interactive Controls**: Slider-based tenure selection with immediate feedback

## Document Management
- **File Upload System**: Support for document uploads with progress tracking
- **Document Types**: Structured handling for different document categories
- **Validation**: File type and size validation for uploaded documents

## User Experience Features
- **Progress Tracking**: Visual stepper component showing current position in application flow
- **Mobile Verification**: Integrated mobile number verification with loading states
- **Selection Interface**: Toggle-based selection for loan types and employment categories
- **Conditional Logic**: Smart form behavior that shows/hides sections based on user selections

# External Dependencies

## Core Technologies
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with Flexbox/Grid layouts
- **Icons/UI**: Custom styled components (no external UI frameworks)

## Potential Integrations
- **SMS Gateway**: For mobile number verification (implementation ready)
- **Document Storage**: File upload system prepared for backend integration
- **Payment Gateway**: Architecture supports future payment processing integration
- **Credit Scoring API**: Structure allows for external credit assessment services
- **Bank APIs**: Framework ready for bank-specific loan processing integrations

## Browser APIs
- **Local Storage**: For form data persistence
- **File API**: For document upload handling
- **Fetch API**: Prepared for future backend communication

Note: The current implementation is frontend-focused with backend-ready architecture for seamless integration with loan processing APIs and databases.