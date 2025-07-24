# Sanad

A healthcare mobile application developed by The Egyptian Society of Rheumatic Diseases (ESRd) to support patients and healthcare professionals in managing rheumatic diseases.

## Overview

Sanad (Arabic for "support") is a comprehensive mobile health application designed to provide essential services and resources for patients with rheumatic diseases. Developed by The Egyptian Society of Rheumatic Diseases, the app serves as a digital platform connecting patients with healthcare providers while offering various tools for disease management and community support.

## Features

### Core Functionality
- **Patient Registration & Authentication** - Secure account creation and login system
- **Social Media Integration** - Login with Facebook, X (Twitter), and other social platforms
- **User Profiles** - Personalized patient profiles with medical information
- **Location-Based Services** - Find nearby healthcare providers and medical facilities
- **Payment Integration** - Secure payment processing via Fawry platform

### Communication & Community
- **User-to-User Communication** - Connect with other patients and healthcare professionals
- **Push Notifications** - Important health reminders and updates
- **Support Groups** - Community features for patient interaction and support

### Health Management
- **Medical Records Management** - Store and manage personal health information
- **Appointment Scheduling** - Book and manage medical appointments
- **Health Tracking** - Monitor symptoms and treatment progress
- **Educational Resources** - Access to rheumatic disease information and guidelines

### Technical Features
- **Offline Capability** - Core features available without internet connection
- **Data Synchronization** - Secure cloud sync across devices
- **Multi-language Support** - Available in Arabic and English
- **Accessibility Features** - Designed for users with mobility limitations

## Tech Stack

### Mobile Framework
- **Flutter** - Cross-platform mobile development framework
- **Dart** - Programming language for Flutter applications

### Backend & Services
- **Cloud Storage** - Secure data storage and backup
- **Google Maps API** - Location services and mapping
- **Google Analytics** - User behavior analysis and app performance monitoring
- **Fawry Payment Gateway** - Payment processing for Egyptian market

### Authentication & Social
- **Firebase Authentication** (inferred) - User management and authentication
- **Facebook SDK** - Social media login integration
- **Twitter SDK** - Social media login integration

### Development Tools
- **Android Studio/VS Code** - Development environment
- **Git** - Version control system
- **Firebase Console** - Backend management

## Installation

### Prerequisites
- Flutter SDK (version 3.0.0 or higher)
- Dart SDK (version 2.17.0 or higher)
- Android Studio or VS Code with Flutter extensions
- Android SDK for Android development
- Xcode for iOS development (macOS only)

### Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/esrd/sanad-mobile.git
   cd sanad-mobile
   ```

2. **Install Flutter dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure environment variables**
   ```bash
   cp .env.example .env
   # Edit .env file with your API keys and configuration
   ```

4. **Set up Firebase**
   - Download `google-services.json` for Android
   - Download `GoogleService-Info.plist` for iOS
   - Place files in respective platform directories

5. **Run the application**
   ```bash
   # For development
   flutter run
   
   # For specific platform
   flutter run -d android
   flutter run -d ios
   ```

### Production Build

```bash
# Android APK
flutter build apk --release

# Android App Bundle
flutter build appbundle --release

# iOS
flutter build ios --release
```

## Usage

### For Patients
1. **Registration**: Create an account using email or social media
2. **Profile Setup**: Complete medical history and personal information
3. **Find Providers**: Use location services to find nearby rheumatologists
4. **Book Appointments**: Schedule appointments with healthcare providers
5. **Track Health**: Monitor symptoms and medication adherence
6. **Connect**: Join support groups and communicate with other patients

### For Healthcare Providers
1. **Professional Registration**: Verify credentials and create provider profile
2. **Patient Management**: Access patient records and treatment history
3. **Appointment Management**: Manage scheduling and availability
4. **Medical Documentation**: Update patient records and treatment plans
5. **Communication**: Secure messaging with patients

## Folder Structure

```
sanad/
├── android/                    # Android-specific files
├── ios/                        # iOS-specific files
├── lib/                        # Main application code
│   ├── main.dart              # App entry point
│   ├── models/                # Data models
│   ├── services/              # API and business logic
│   ├── screens/               # UI screens
│   ├── widgets/               # Reusable UI components
│   ├── utils/                 # Helper functions
│   └── constants/             # App constants
├── assets/                     # Images, fonts, and other assets
├── test/                       # Unit and widget tests
├── integration_test/           # Integration tests
├── content/                    # Documentation and legal content
│   └── index.html             # Privacy policy
├── pubspec.yaml               # Dependencies and metadata
├── README.md                  # Project documentation
└── .env                       # Environment variables
```

## Privacy & Security

The Sanad app is committed to protecting user privacy and maintaining the highest security standards:

- **HIPAA Compliance** - Follows healthcare data protection standards
- **GDPR Compliance** - Meets European data protection requirements
- **Data Encryption** - All sensitive data encrypted in transit and at rest
- **Secure Authentication** - Multi-factor authentication available
- **Privacy Controls** - Users control their data sharing preferences

For detailed privacy information, see our [Privacy Policy](content/index.html).

## Contributing

We welcome contributions from the developer community! Please follow these guidelines:

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow Flutter/Dart style guide
- Write comprehensive tests for new features
- Update documentation for API changes
- Ensure HIPAA compliance for health-related features

### Code Review Process
- All changes require review by core team members
- Automated tests must pass
- Security review required for authentication/payment features

---

## Contact & Support

**The Egyptian Society of Rheumatic Diseases (ESRd)**
- **Website**: [www.esrdeg.com](http://www.esrdeg.com)
- **Email**: info@esrdeg.com
- **Support**: For technical support and bug reports, please open an issue in this repository

---

*Sanad - Supporting the rheumatic disease community through technology* 