# MIU Tech

This is a side project and not used in the university

## Documentation

- 📊 [Project Presentation (PDF)](https://raw.githubusercontent.com/ismailtaha12/MOBILE-PROJECT-UNI_TECH/main/docs/MIU-TechCircle-Presentation.pdf)
- 🏛️ [Software Architecture (PDF)](https://raw.githubusercontent.com/ismailtaha12/MOBILE-PROJECT-UNI_TECH/main/docs/SW-Architecture-Project.pdf)

A Flutter-based social and collaboration platform built for the MIU university community. The app combines a social feed, stories, messaging, freelancing hub, announcements, calendar events, and administrative tools in a single cross-platform mobile experience.



## Features

- **Authentication** — Email/password signup, email verification, password reset (OTP), and Google Sign-In.
- **Social Feed** — Create posts with images/videos, comment, like, save, and repost.
- **Stories** — 24-hour stories with viewer tracking and a dedicated player.
- **Messaging** — Private chat rooms with per-chat settings.
- **Friendships** — Friend requests, follow/unfollow, and profile discovery.
- **Freelancing Hub** — Post projects, submit applications, and manage candidates.
- **Announcements & Opportunities** — Admin-curated posts for the community.
- **Calendar** — Integrated Google Calendar events and `add_2_calendar` support.
- **Notifications** — In-app notifications with user-configurable preferences.
- **Admin Panel** — Manage users, posts, reports, feedback, applications, announcements, and more.
- **Search** — Global search across posts, users, and tags.
- **Profiles** — Editable profile with avatar upload 

## Tech Stack

- **Flutter** (SDK ≥ 3.8.1)
- **Supabase** — Auth, database, and realtime backend
- **Cloudinary** — Media storage for images/videos
- **Riverpod** + **Provider** — State management
- **Google APIs** — Sign-In and Calendar integration
- **flutter_animate**, **google_fonts**, **confetti** — UI polish



## Project Structure

```
lib/
├── main.dart              # App entry point & provider setup
├── app_theme.dart         # Global theme
├── controllers/           # Business logic controllers
├── models/                # Data models (posts, users, stories, etc.)
├── providers/             # Riverpod/Provider state
├── services/              # Supabase, Cloudinary, Google, AI services
├── utils/                 # Helpers and utilities
└── views/
    ├── screens/           # ~50 app screens (auth, feed, chat, admin, …)
    └── widgets/           # Reusable UI components
```

## Getting Started

### Prerequisites

- Flutter SDK `>=3.8.1 <4.0.0`
- Dart SDK bundled with Flutter
- A Supabase project (URL + anon key)
- Google OAuth credentials (for Sign-In and Calendar)

### Setup

1. **Clone the repo**
   ```bash
   git clone <repo-url>
   cd miu_tech
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Create a `.env` file** in the project root:
   ```env
   SUPABASE_URL=your_supabase_url
   SUPABASE_ANON_KEY=your_supabase_anon_key

   ```

4. **Run the app**
   ```bash
   flutter run
   ```

## Supported Platforms

Android · iOS · Web · Windows · macOS · Linux

## Scripts

```bash
flutter pub get          # Install packages
flutter run              # Launch on a connected device
```

## License

This project is part of a university course and is not published to pub.dev.
