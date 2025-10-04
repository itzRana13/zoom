# Yoom - Video Calling App

A modern video calling application built with Next.js, featuring real-time video calls, meeting scheduling, and user authentication.

## 🚀 Live Demo

**Production URL:** https://zoom-p1x6ah70e-itzrana13s-projects.vercel.app

## ✨ Features

- 🎥 Real-time video calling with Stream.io
- 🔐 User authentication with Clerk
- 📅 Meeting scheduling and management
- 👥 Personal meeting rooms
- 📱 Responsive design for all devices
- 🎨 Modern UI with Tailwind CSS

## 🛠️ Tech Stack

- **Frontend:** Next.js 14, React 18, TypeScript
- **Authentication:** Clerk
- **Video SDK:** Stream.io
- **Styling:** Tailwind CSS, Radix UI
- **Deployment:** Vercel

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- npm, yarn, pnpm, or bun
- Clerk account for authentication
- Stream.io account for video features

### Installation

1. Clone the repository:
```bash
git clone https://github.com/itzRana13/zoom.git
cd zoom
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
```

4. Add your environment variables to `.env.local`:
```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
CLERK_SECRET_KEY=your_clerk_secret_key_here

# Stream.io Video SDK
NEXT_PUBLIC_STREAM_API_KEY=your_stream_api_key_here
STREAM_SECRET_KEY=your_stream_secret_key_here
```

5. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

6. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🔧 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY` | Clerk publishable key | Yes |
| `CLERK_SECRET_KEY` | Clerk secret key | Yes |
| `NEXT_PUBLIC_STREAM_API_KEY` | Stream.io API key | Yes |
| `STREAM_SECRET_KEY` | Stream.io secret key | Yes |

## 📦 Deployment

### Deploy to Vercel

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Deploy to production:
```bash
vercel --prod
```

3. Add environment variables in Vercel dashboard:
   - Go to your project settings
   - Navigate to Environment Variables
   - Add all required variables for Production environment

### Manual Deployment

1. Build the application:
```bash
npm run build
```

2. Start the production server:
```bash
npm start
```

## 🎯 Project Structure

```
zoom/
├── app/                    # Next.js app directory
│   ├── (auth)/            # Authentication pages
│   ├── (root)/            # Main application pages
│   └── globals.css        # Global styles
├── components/            # Reusable components
│   ├── ui/               # UI components
│   └── ...               # Feature components
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions
├── providers/            # Context providers
└── public/               # Static assets
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) for the amazing framework
- [Clerk](https://clerk.com/) for authentication
- [Stream.io](https://getstream.io/) for video SDK
- [Vercel](https://vercel.com/) for deployment platform
