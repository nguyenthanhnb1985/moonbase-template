# 🚀 Moonbase

A complete Flutter social media template with authentication, moderation, and monetization

Show Image
Show Image
Show Image
✨ Features
🔐 Authentication - Email, Google & Apple Sign-In
📱 Social Platform - Posts, comments, categories
🛡️ Content Moderation - User blocking & reporting
💰 Subscriptions - RevenueCat integration
🏗️ Clean Architecture - BLoC pattern & repository design
📸 Screenshots
Coming soon...
🚀 Quick Start
Prerequisites

Flutter 3.0+
Firebase project

Setup

Clone the repository
bashgit clone https://github.com/mitchkoko/moonbase-template.git
cd moonbase-template
flutter pub get

Configure Firebase

Create project at Firebase Console
Add your app and download config files
Enable Authentication & Firestore
Uncomment Firebase initialization in main.dart


Run the app
bashflutter run


Optional: RevenueCat Setup
Replace the API key in lib/features/subscriptions/data/revenuecat_constants.dart
🏗️ Architecture
lib/
├── features/
│   ├── auth/           # Authentication
│   ├── home/          # Posts & comments  
│   ├── moderation/    # User blocking
│   └── subscriptions/ # Monetization
├── components/        # Shared UI
└── themes/           # Light/dark themes
Built with Clean Architecture principles and BLoC state management.
🎨 Customization

Themes: Edit themes/light_mode.dart and themes/dark_mode.dart
Categories: Modify tabs in home_page.dart
Colors: Update ColorScheme in theme files

📱 Platform Support
✅ iOS
✅ Android
❌ Web (Firebase Auth limitations)
🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

Built by Mitch Koko