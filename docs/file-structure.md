# Project File Structure

```bash
/my-workout-tracker
├── app/                     # Next.js App Router (UI)
│   ├── page.tsx            # Homepage
│   ├── api/                # Next.js API routes (simple logic)
│   │   ├── auth/route.ts   # Login, register
│   │   ├── workouts/       # Simple read/write routes
│   │   │   └── route.ts
│   │   └── cache/          # Cache fetch example
│   │       └── route.ts
│   └── dashboard/          # Authenticated user dashboard
│       └── page.tsx
│
├── lambdas/                # AWS Lambda functions (heavy/complex logic)
│   ├── analyzeWorkout.js   # Example: complex analytics
│   ├── generatePDF.js      # Example: PDF generation
│   └── notifyUsers.js      # Example: email scheduler
│
├── lib/                    
│   ├── db.js               # DB connection (MongoDB/DynamoDB)
│   ├── redis.js            # Redis cache connector
│   └── apiClient.js        # Wrapper to call Lambda functions
│
├── public/                 # Static files
├── styles/                 # Global CSS
├── .env.local              # Local env vars
├── next.config.js
├── package.json
└── README.md
```