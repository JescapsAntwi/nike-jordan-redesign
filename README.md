# Nike Redesign - E-Commerce Website

![Project Banner](/screenshott.png) <!-- Replace with your actual banner image -->

A modern redesign of the Nike e-commerce website built with Next.js, TypeScript, Tailwind CSS, and Firebase. This project features a responsive design, product catalog, authentication, and more.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Setup](#setup)
- [Environment Variables](#environment-variables)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Modern UI/UX**: Redesigned Nike interface with smooth animations
- **Responsive Design**: Works on mobile, tablet, and desktop
- **Product Catalog**: Browse shoes, apparel, and accessories
- **Authentication**: User sign-up/login with Firebase Auth
- **Shopping Cart**: Add/remove items and manage quantities
- **Search Functionality**: Find products quickly
- **Order History**: View past purchases
- **Admin Dashboard**: Manage products and orders (if implemented)

## Technologies

- **Frontend**:
  - Next.js (App Router)
  - TypeScript
  - Tailwind CSS
  - Framer Motion (for animations)
  - React Icons

- **Backend**:
  - Firebase Authentication
  - Firestore Database
  - Firebase Storage
  - Firebase Hosting (optional)

- **Testing**:
  - Jest
  - React Testing Library

## Project Structure

```
nike-redesign/
├── public/                  # Static files
│   ├── images/              # Product images and assets
│   └── favicon.ico          # Website favicon
│
├── src/
│   ├── app/                 # Next.js app router
│   │   ├── (auth)/          # Authentication routes
│   │   ├── (main)/          # Main application routes
│   │   ├── api/             # API routes
│   │   ├── cart/            # Cart related pages
│   │   ├── product/         # Product pages
│   │   ├── layout.tsx       # Root layout
│   │   └── page.tsx         # Home page
│   │
│   ├── components/          # Reusable components
│   │   ├── ui/              # UI primitives (buttons, inputs)
│   │   ├── cart/            # Cart components
│   │   ├── product/         # Product components
│   │   ├── Header.tsx       # Main navigation
│   │   └── Footer.tsx       # Site footer
│   │
│   ├── context/             # React contexts
│   │   ├── AuthContext.tsx  # Authentication state
│   │   └── CartContext.tsx  # Shopping cart state
│   │
│   ├── hooks/               # Custom hooks
│   │   ├── useAuth.ts       # Authentication hook
│   │   └── useCart.ts       # Cart management hook
│   │
│   ├── lib/                 # Utility functions
│   │   ├── firebase/        # Firebase configuration
│   │   ├── constants.ts     # App constants
│   │   └── utils.ts         # Helper functions
│   │
│   ├── styles/              # Global styles
│   │   └── globals.css      # Tailwind imports
│   │
│   ├── types/               # TypeScript types
│   │   ├── product.ts       # Product type definitions
│   │   └── user.ts          # User type definitions
│   │
│   └── assets/              # Design assets (SVGs, etc.)
│
├── .env.local               # Environment variables
├── next.config.js           # Next.js configuration
├── tailwind.config.js       # Tailwind configuration
├── tsconfig.json            # TypeScript configuration
├── package.json             # Project dependencies
└── README.md                # This file
```

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/nike-jordan-redesign.git
   cd nike-jordan-redesign
   ```

2. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up Firebase:
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Authentication (Email/Password)
   - Set up Firestore Database
   - Set up Storage for product images

4. Run the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   ```

## Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=your-api-key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your-project-id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your-bucket.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your-sender-id
NEXT_PUBLIC_FIREBASE_APP_ID=your-app-id
NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID=your-measurement-id
```

## Deployment

To deploy to Vercel:

1. Push your code to a GitHub repository
2. Import the project in Vercel
3. Add your Firebase environment variables
4. Deploy!

For Firebase Hosting:

```bash
npm run build
firebase init hosting
firebase deploy
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

## Project History

This Nike redesign website was originally created by [Miren Savani](https://github.com/mirensavani) and subsequently modified and enhanced by [Jescaps Antwi](https://github.com/jescapsantwi).

### Original Work

- Initial architecture and core functionality by Miren Savani
- Base implementation using Next.js, TypeScript, and Tailwind CSS
- Foundational Firebase integration for authentication and data storage

### Modifications & Enhancements

- Implemented new UI components for improved user experience
- Enhanced performance through [specific optimizations]
- Added [specific new features] functionality
- Refactored [specific aspects] for better maintainability
- Extended Firebase integration to include [new features]

### Acknowledgments

Special thanks to Miren Savani for the original work that served as the foundation for this project.

### Development Approach

- **Modern Stack**: Leveraged Next.js for server-side rendering and static generation, TypeScript for type safety, and Tailwind CSS for rapid UI development
- **Performance Focus**: Implemented code splitting, image optimization, and efficient state management
- **Firebase Integration**: Utilized Firebase Auth for secure authentication and Firestore for real-time data synchronization
- **Mobile-First**: Designed with a responsive approach to ensure optimal experience across all devices

### Contact

- Portfolio: [jesantwi.vercel.app]()
- GitHub: [github.com/jescapsantwi]()
- LinkedIn: [linkedin.com/in/jescapsantwi]()
- Email: <antwijescaps1@gmail.com>

Feel free to reach out for collaboration opportunities or feedback on this project!

**Note**: This is a redesign project for educational purposes only. All Nike branding, logos, and product images are property of Nike, Inc.
