🚀 Moonbase - Flutter Social Media Template

A complete Flutter social media app template with authentication, content moderation, and subscription monetization.

✨ Features

🔐 Authentication: Email/password, Google Sign-In, Apple Sign-In
📱 Social Platform: Posts, comments, categories (Build, Launch, Monetize)
🛡️ Content Moderation: User blocking, content reporting, safety features
💰 Pro Subscriptions: RevenueCat integration for premium features
🏗️ Clean Architecture: BLoC state management, repository pattern

📸 Screenshots
Add screenshots here once you have them
🚀 Quick Start
Prerequisites

Flutter 3.0+
Dart 3.0+
Firebase project
(Optional) RevenueCat account for subscriptions

1. Clone & Install
bashgit clone https://github.com/yourusername/moonbase-template.git
cd moonbase-template
flutter pub get
2. Firebase Setup

Create a Firebase project at console.firebase.google.com
Add your Flutter app to the project
Download and add configuration files:

Android: google-services.json → android/app/
iOS: GoogleService-Info.plist → ios/Runner/


Enable Authentication providers (Email/Password, Google, Apple)
Create Firestore database
In main.dart, uncomment these lines:
dartawait Firebase.initializeApp(options: DefaultFirebaseOptions.currentPlatform);
firebaseInitialized = true;


3. RevenueCat Setup (Optional)

Create account at revenuecat.com
Set up your products and entitlements
Replace YOUR_REVENUECAT_API_KEY_HERE in lib/features/subscriptions/data/revenuecat_constants.dart

4. Run the App
bashflutter run
📁 Project Structure
lib/
├── components/           # Shared UI components
├── features/
│   ├── auth/            # Authentication (login, register, etc.)
│   ├── home/            # Posts and comments
│   ├── moderation/      # User blocking and reporting
│   └── subscriptions/   # RevenueCat integration
└── themes/              # Light and dark themes
🏗️ Architecture
This app follows Clean Architecture principles:

Domain Layer: Entities and repository interfaces
Data Layer: Firebase implementations and data sources
Presentation Layer: UI components and BLoC state management

🔧 Customization
Adding New Post Categories

Update the tab names in home_page.dart
Modify the category logic in the addPost() method

Changing App Theme
Edit themes/light_mode.dart and themes/dark_mode.dart
Adding New Features
Follow the existing feature structure in the features/ directory
📱 Supported Platforms

✅ iOS
✅ Android
❌ Web (Firebase Auth limitations)
❌ Desktop (not optimized)

🤝 Contributing

Fork the repository
Create a feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments

Flutter team for the amazing framework
Firebase for backend services
RevenueCat for subscription management

📞 Support

Create an issue for bug reports
Discussions for questions and feature requests
Follow @mitchkoko for updates


Built with ❤️ by Mitch Koko