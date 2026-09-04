# Pet First-Aid Web Application
This is our group project for SWE30003 Software Architectures and Design at Swinburne University Sarawak. Group 25.
The web application is built for a Veterinary Association to help pet owners get fast and reliable first aid information for their pets.

## Group Members

- Wei Chien CHIN (104401173)
- Jun Zhen WONG (104385730)
- Aeron Yun Chiang LIU (102769264)
- Aaric Ching Chian LEE (104390404)
- Umer NASEER (104404127)


## Tech Stack
-Frontend: Next.js 16, React 19, TypeScript, Tailwind CSS
-Backend: Supabase (PostgreSQL)

# Prerequisites
- Node.js installed
- npm or yarn package manager
- Supabase project (for database)

## Getting Started
1. **Clone the repository**
```bash
git clone <repository-url>
cd SoftwareDeployment
```

2. **Install dependencies**
```bash
npm install
```

3. **Configure environment variables**

Create a `.env.local` file in the root directory with the following variables:

```env
# Supabase Configuration
NEXT_PUBLIC_SUPABASE_URL=<your-supabase-url>
NEXT_PUBLIC_SUPABASE_ANON_KEY=<your-supabase-anon-key>
```

## Build for Production

```bash
npm run build
```

## Development

Start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Project Structure

```
app/                   # Next.js App Router pages
├── staff/             # Staff pages (CRUD content, reply enquiry )
├── FirstAidContent/   #  First-aid information pages
├── vet/               # Vet pages (first-aid content decision, reply enquiry)
├── enquiry/           # enquiry page (ask question)
├── emergency/         # emergency page (shows nearby clinic)
├── dashboard/         # dashboard page (showing first-aid service)
├── login/             # product page
├── profile/           # profile page
└── page.tsx           # homepage

components/            # React components
├── navbar.tsx             # Header components
└──  sidebar.tsx           # Navigation component 

lib/                   # Utility libraries
├── supabase.ts        # Supabase client configuration           
```

## Key Features
-Homepage with pet first aid information
-User registration and login
-Role based access for Pet Owner, Staff and Veterinarian
-First aid guides, videos and quizzes
-Emergency contact page
-Submit enquiry to staff and veterinarian


## Contributing

This is a university project. Please follow the existing code style and conventions.

## License

This project is for educational purposes as part of Swinburne University's Software Deployment Project.
