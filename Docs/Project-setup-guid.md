# Initialize Next.js project with TypeScript
npx create-next-app@latest . --typescript --tailwind --eslint
# Answer the setup questions:
# ✔ Would you like to use App Router? Yes
# ✔ Would you like to customize the default import alias (@/*)? Ye






# Install Required Dependencies
## Install main dependencies
npm install @prisma/client firebase stripe lucide-react date-fns

## Install development dependencies
npm install -D prisma @types/node

## Install UI components
npm install @/components/ui/button @/components/ui/card @/components/ui/input





#Git



# Environment
## Create .env.local file
cat > .env.local << EOL
## Firebase Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

## Stripe Configuration
STRIPE_SECRET_KEY=your_stripe_secret_key
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key

## MongoDB Configuration
MONGODB_URI=your_mongodb_uri
EOL

# Create Basic Project Structure
## Create necessary directories
mkdir -p src/app/{search,flights,bookings} src/components/{common,flight,payment} src/lib src/api/{search,bookings,webhook/stripe}

## Create basic component files
touch src/components/common/{Navbar,Footer,LoadingSpinner}.tsx
touch src/components/flight/{SearchForm,FlightCard,BookingForm}.tsx
touch src/components/payment/CheckoutForm.tsx

## Create utility files
touch src/lib/{db,firebase,stripe}.ts

## Create API route files
touch src/api/search/route.ts
touch src/api/bookings/route.ts
touch src/api/webhook/stripe/route.ts


# Connect to GitHub
## Create a new repository on GitHub first, then:
git remote add origin https://github.com/yourusername/pickmyflights.git
git branch -M main
git push -u origin main



# Running the Project Locally
## Install dependencies (if not done already)
npm install




# Run development server
npm run dev


