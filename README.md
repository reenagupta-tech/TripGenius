# 🧠 TripGenius — Your Personal AI Travel Planner & Itinerary Generator
Your intelligent travel companion for creating personalized itineraries, discovering destinations, and planning perfect trips with AI-powered recommendations.

**React** **Vite** **Firebase** **Google Gemini** **Tailwind CSS** **License**

## 📌 Overview
TripGenius is a full-stack travel planning application designed to help users create personalized travel itineraries through AI-powered recommendations, manage their trip history, and discover amazing destinations tailored to their preferences and budget.

## 📖 Repository: https://github.com/reena001/tripgenius

## ✨ Features

### 🗺️ AI-Powered Trip Planning
- **Intelligent Itinerary Generation** using Google Gemini AI
- **Personalized Recommendations** based on destination, budget, and travel preferences
- **Real-time AI Chat** for travel planning assistance
- **Context-aware suggestions** for hotels, attractions, and activities

### 🏨 Hotel & Accommodation Management
- **Curated Hotel Options** with detailed information
- **Price filtering** based on budget preferences (Cheap, Moderate, Luxury)
- **Hotel ratings, descriptions, and images** for informed decisions
- **Geographic coordinates** for easy navigation

### 🎯 Smart Travel Preferences
- **Destination Selection** with Google Places Autocomplete
- **Travel Duration Planning** (1-30+ days)
- **Budget Categories** (Cheap, Moderate, Luxury)
- **Traveler Types** (Solo, Couple, Family, Friends)

### 📱 Trip Management & History
- **Personal Trip Library** with all generated itineraries
- **Trip History Tracking** with detailed information
- **Easy Trip Access** and modification capabilities
- **User-specific trip storage** with Firebase

### 🔐 User Authentication
- **Google OAuth Integration** for secure login
- **User session management** with localStorage
- **Protected trip access** for authenticated users
- **Seamless authentication flow**

### 🎨 Modern UI/UX
- **Responsive Design** for all devices
- **Beautiful Landing Page** with hero section
- **Interactive Components** with smooth animations
- **Tailwind CSS** for modern styling

## 🛠️ Tech Stack

| Frontend | Backend | Database | AI Integration | Authentication |
|----------|---------|----------|----------------|----------------|
| React + Vite | Firebase | Firestore | Google Gemini API | Google OAuth |

## 🏗️ Project Structure

```
TripGenius/
├── 📁 public/                    # Static assets
│   ├── 📁 asset/                 # Project images and assets
│   ├── 📄 landing.png            # Landing page hero image
│   └── 📄 logo.svg               # Application logo
│
├── 📁 src/                       # Source code
│   ├── 📁 components/            # Reusable UI components
│   │   ├── 📁 custom/            # Custom components
│   │   │   ├── 📄 Header.jsx     # Navigation header
│   │   │   └── 📄 Hero.jsx       # Landing page hero
│   │   └── 📁 ui/                # UI component library
│   │       ├── 📄 button.jsx     # Button components
│   │       ├── 📄 dialog.jsx     # Modal dialogs
│   │       ├── 📄 input.jsx      # Input fields
│   │       ├── 📄 popover.jsx    # Popover components
│   │       └── 📄 sonner.jsx     # Toast notifications
│   │
│   ├── 📁 constants/             # Application constants
│   │   └── 📄 options.jsx        # Travel options and AI prompts
│   │
│   ├── 📁 create-trip/           # Trip creation functionality
│   │   └── 📄 index.jsx          # Main trip creation page
│   │
│   ├── 📁 my-trips/              # Trip management
│   │   ├── 📁 components/        # Trip-related components
│   │   │   └── 📄 UserTripCardItem.jsx  # Trip card component
│   │   └── 📄 index.jsx          # My trips page
│   │
│   ├── 📁 service/               # External services
│   │   ├── 📄 AIModel.jsx        # Google Gemini AI integration
│   │   ├── 📄 firebaseConfig.jsx # Firebase configuration
│   │   └── 📄 GlobalApi.jsx      # Global API utilities
│   │
│   ├── 📁 view-trip/             # Trip viewing functionality
│   │   ├── 📁 [tripId]/          # Dynamic trip routes
│   │   │   └── 📄 index.jsx      # Individual trip view
│   │   └── 📁 components/        # Trip view components
│   │       ├── 📄 Footer.jsx     # Application footer
│   │       ├── 📄 HotelCardItem.jsx  # Hotel display component
│   │       ├── 📄 Hotels.jsx     # Hotels section
│   │       ├── 📄 InfoSection.jsx # Trip information
│   │       ├── 📄 PlaceCardItem.jsx  # Place display component
│   │       └── 📄 PlacesToVisit.jsx  # Places section
│   │
│   ├── 📁 lib/                   # Utility libraries
│   │   └── 📄 utils.js           # Helper functions
│   │
│   ├── 📄 App.jsx                # Main application component
│   ├── 📄 main.jsx               # Application entry point
│   └── 📄 index.css              # Global styles
│
├── 📄 package.json               # Dependencies and scripts
├── 📄 vite.config.js             # Vite configuration
├── 📄 tailwind.config.js         # Tailwind CSS configuration
├── 📄 postcss.config.js          # PostCSS configuration
└── 📄 README.md                  # Project documentation
```

## 🛠️ Setup & Installation

Make sure Node.js and npm are installed before proceeding.

### 🔹 Step 1: Clone the Repository
```bash
git clone https://github.com/reena001/tripgenius.git
cd tripgenius
```

### 🔹 Step 2: Install Dependencies
```bash
npm install
```

### 🔹 Step 3: Setup Environment Variables
Create a `.env` file in the root directory:

```env
# Google Gemini AI API Key
VITE_GOOGLE_GEMINI_AI_API_KEY=your_gemini_api_key_here

# Google Places API Key
VITE_GOOGLE_PLACE_API_KEY=your_google_places_api_key_here

# Firebase Configuration (if using custom Firebase project)
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
VITE_FIREBASE_PROJECT_ID=your_firebase_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
VITE_FIREBASE_APP_ID=your_firebase_app_id
```

### 🔹 Step 4: Run the Development Server
```bash
npm run dev
```

### 🔹 Step 5: Visit the App
Open your browser at:
📍 **http://localhost:5173** (TripGenius frontend)

## 📱 Screenshots

### Landing Page
![Landing Page](https://github.com/reena001/tripgenius/blob/main/public/asset/1.1.png)

### Google OAuth Sign in
![Google OAuth Sign in](https://github.com/reena001/tripgenius/blob/main/public/asset/2.png)

### Create Trip Page
![Create Trip Page](https://github.com/reena001/tripgenius/blob/main/public/asset/4.4.png)

### View Trip Page: AI-generated Hotel Recommendations & Places to Visit
![View Trip Page: AI-generated Hotel Recommendations & Places to Visit](https://github.com/reena001/tripgenius/blob/main/public/asset/7.png)

### My Trips Page
![My Trips Page](https://github.com/reena001/tripgenius/blob/main/public/asset/6.png)

### Responsive view on mobile
![Responsive view on mobile](https://github.com/reena001/tripgenius/blob/main/public/asset/8.jpg)


## 👨‍💻 Author

**Reena Gupta**
- GitHub: [@reena001](https://github.com/reena001)
- LinkedIn: [Reena Gupta](https://linkedin.com/in/reena-gupta)

---

Made with ❤️ by **Reena Gupta**
