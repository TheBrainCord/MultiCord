pickmyflights.com/
├── src/
│   ├── app/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── search/
│   │   │   └── page.tsx
│   │   ├── flights/
│   │   │   └── [id]/
│   │   │       └── page.tsx
│   │   └── bookings/
│   │       └── page.tsx
│   ├── components/
│   │   ├── common/
│   │   │   ├── Navbar.tsx
│   │   │   ├── Footer.tsx
│   │   │   └── LoadingSpinner.tsx
│   │   ├── flight/
│   │   │   ├── SearchForm.tsx
│   │   │   ├── FlightCard.tsx
│   │   │   └── BookingForm.tsx
│   │   └── payment/
│   │       └── CheckoutForm.tsx
│   ├── lib/
│   │   ├── db.ts
│   │   ├── firebase.ts
│   │   └── stripe.ts
│   └── api/
│       ├── search/
│       │   └── route.ts
│       ├── bookings/
│       │   └── route.ts
│       └── webhook/
│           └── stripe/
│               └── route.ts
├── public/
│   ├── images/
│   └── icons/
└── package.json

