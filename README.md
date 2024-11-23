# Imaginify - AI Image Manipulation Platform

![Imaginify Banner](/public/dp.png)

## 🌟 Overview

Imaginify is a powerful AI-powered SaaS platform that offers advanced image manipulation features through an intuitive interface. Built with modern technologies, it provides users with AI-powered tools for image enhancement, manipulation, and generation.

## ✨ Features

### Image Manipulation
- 🎨 AI Generative Fill
- 🔄 Image Restoration
- 🎯 Object Removal
- 🖼️ Background Removal
- 🌈 Image Recoloring

### Advanced Search
- 📷 Content-Based Image Search
- 🔍 Search images based on visual content
- 🏷️ Smart tagging and categorization

### User Management
- 👤 Secure Authentication via Clerk
- 💳 Credit-based system
- 📊 User dashboard with usage statistics

### Payment Integration
- 💰 Secure payments via Stripe
- 💳 Multiple pricing plans
- 🔄 Automatic credit renewal

## 🛠️ Technologies Used

- **Frontend**:
  - Next.js 14 (App Router)
  - TypeScript
  - Tailwind CSS
  - Shadcn UI Components

- **Backend**:
  - MongoDB (Database)
  - Cloudinary API (Image Processing)
  - Clerk (Authentication)
  - Stripe (Payments)

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ installed
- MongoDB database
- Cloudinary account
- Clerk account
- Stripe account

### Environment Variables

Create a `.env.local` file in the root directory:

```env
# MongoDB
MONGODB_URL=your_mongodb_url

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# Cloudinary
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Stripe
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
```

### Installation

1. Clone the repository:
```bash
git clone https://https://github.com/adeektya/imaginify
cd imaginify
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📁 Project Structure

```
imaginify/
├── app/
│   ├── (auth)/
│   │   ├── sign-in/
│   │   └── sign-up/
│   ├── (root)/
│   │   ├── credits/
│   │   ├── profile/
│   │   └── transformations/
│   └── layout.tsx
├── components/
│   ├── shared/
│   └── ui/
├── lib/
│   ├── actions/
│   ├── database/
│   └── utils/
├── public/
└── next.config.js
```

## 💳 Credits System

- Users start with free credits
- Additional credits can be purchased
- Credits are consumed for each image transformation
- Real-time credit balance tracking

## 🔒 Authentication Flow

1. User signs up/logs in using Clerk
2. User profile is created in MongoDB
3. Credit balance is initialized
4. Access to transformation features is granted

## 🖼️ Image Transformation Process

1. User uploads image
2. Image is processed through Cloudinary
3. AI models apply selected transformations
4. Transformed image is saved and displayed
5. Credits are deducted from user balance

## 💰 Payment Processing

1. User selects credit package
2. Stripe checkout is initiated
3. Payment is processed securely
4. Credits are added to user account
5. Transaction is recorded in database

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 🙏 Acknowledgments

- Next.js Team
- Cloudinary Team
- Shadcn UI
- MongoDB Team
- Stripe Team
- Clerk Team