# Vehiql – AI Car Marketplace

Vehiql is a full-stack AI-powered car marketplace built with Next.js, Supabase, Prisma, Clerk, Tailwind CSS, ArcJet, and Shadcn UI. It enables users to browse, search, and book test drives for vehicles, while providing dealerships with powerful inventory management and AI-driven tools for car detail extraction.

<img width="1277" height="606" alt="Screenshot (126)" src="https://github.com/user-attachments/assets/71d210b8-d82e-42ed-aceb-3fcd770de74e" />
<img width="1289" height="615" alt="Screenshot (127)" src="https://github.com/user-attachments/assets/406ef18f-9017-47e2-9b7b-30bfe0377da1" />
<img width="1239" height="588" alt="Screenshot (128)" src="https://github.com/user-attachments/assets/08939f1c-4d29-49a3-aae9-a2c792c1c409" />
<img width="1275" height="592" alt="Screenshot (129)" src="https://github.com/user-attachments/assets/9dc341be-da7c-45bc-b70d-19215f24df87" />
<img width="1275" height="621" alt="Screenshot (130)" src="https://github.com/user-attachments/assets/7067f740-9ed1-4d4b-a33e-9b3345bdc82a" />
<img width="1315" height="628" alt="Screenshot (131)" src="https://github.com/user-attachments/assets/92a04e76-2544-4a9c-8c94-01634ba25918" />
<img width="1487" height="712" alt="Screenshot (132)" src="https://github.com/user-attachments/assets/d92e0efb-ee12-41e3-b2a1-a957a6483280" />

---

## Live Url
- https://ai-car-marketplace-two.vercel.app/

---



## Features

- **Modern Car Marketplace**: Browse, search, and filter thousands of verified vehicles from trusted dealerships and private sellers.
- **AI-Powered Car Detail Extraction**: Upload a car image and let Gemini AI extract make, model, year, color, and more.
- **Test Drive Booking**: Book test drives online with flexible scheduling and instant confirmation.
- **User Authentication**: Secure sign-up and sign-in flows powered by Clerk.
- **Admin Dashboard**: Manage inventory, dealership info, working hours, and user roles.
- **Wishlist**: Save favorite cars for quick access.
- **Responsive UI**: Clean, modern, and mobile-friendly interface using Tailwind CSS and Shadcn UI components.

## Tech Stack

- **Frontend**: Next.js (App Router), React, Tailwind CSS, Shadcn UI
- **Backend**: Next.js API routes, Prisma ORM, Supabase (for storage)
- **Authentication**: Clerk
- **AI Integration**: Google Gemini API
- **Other**: ArcJet (security), Sonner (notifications)

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- Bun (optional, for faster installs)
- Supabase account (for image storage)
- Clerk account (for authentication)
- Google Gemini API key
- ArcJet API key

### Installation

1. **Clone the repository**
   ```sh
   git clone https://github.com/your-username/ai-car-marketplace-main.git
   cd ai-car-marketplace-main
   ```

2. **Install dependencies**
   ```sh
   npm install
   # or
   bun install
   ```

3. **Configure environment variables**

   Create a `.env` file in the root directory and add the following:
   ```
   DATABASE_URL=
   DIRECT_URL=

   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
   CLERK_SECRET_KEY=
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

   GEMINI_API_KEY=

   ARCJET_KEY=
   ```

4. **Set up the database**
   ```sh
   npx prisma migrate dev
   ```

5. **Run the development server**
   ```sh
   npm run dev
   # or
   bun run dev
   ```

   The app will be available at [http://localhost:3000](http://localhost:3000).

## Project Structure

- `/app` – Next.js app directory (routes, pages, layouts)
- `/components` – Reusable UI components
- `/actions` – Server actions (database, AI, business logic)
- `/hooks` – Custom React hooks
- `/lib` – Utilities, helpers, and data
- `/prisma` – Prisma schema and migrations
- `/public` – Static assets

## Customization

- **Tailwind CSS**: Customize theme in [`tailwind.config.mjs`](tailwind.config.mjs)
- **Prisma Models**: Update schema in [`prisma/schema.prisma`](prisma/)
- **Supabase Storage**: Configure bucket for car images
- **AI Integration**: Update Gemini API usage in [`actions/home.js`](actions/home.js)

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements and bug fixes.

## License

This project is licensed under the MIT License.

---


**Author**: Mohd Fazal Khan
