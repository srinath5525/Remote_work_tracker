# Remote_work_tracker
# 📱 Remote Work Tracker

A modern, feature-rich Flutter application designed to help remote workers manage their tasks, track productivity, and maintain work-life balance with beautiful UI and offline capabilities.

![Flutter](https://img.shields.io/badge/Flutter-3.8.1-blue)
![Firebase](https://img.shields.io/badge/Firebase-Enabled-orange)
![Offline Support](https://img.shields.io/badge/Offline-Supported-green)
![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS%20%7C%20Web-lightgrey)

## ✨ Features

### 🎯 **Task Management**
- **Create, edit, and delete tasks** with rich descriptions
- **Priority levels** (Low, Medium, High) with color-coded indicators
- **Due date management** with visual countdown
- **Task completion tracking** with completion timestamps
- **Smart filtering** (All, Completed, Overdue, Today)
- **Search functionality** to quickly find tasks

### 📊 **Productivity Dashboard**
- **Visual statistics** showing completed, uncompleted, and overdue tasks
- **Monthly productivity charts** with beautiful bar graphs
- **Real-time updates** as tasks are completed
- **Bold, shadow-enhanced numbers** for better visibility

### 🔄 **Offline Support**
- **Full offline functionality** - work without internet connection
- **Automatic data synchronization** when connection is restored
- **Local caching** with Hive for instant access
- **Pending sync indicators** showing queued changes
- **Network status indicators** in the UI

### 🎨 **Beautiful UI/UX**
- **Frost glass effects** throughout the application
- **Transparent white backgrounds** with blur effects
- **Modern card-based design** with smooth animations
- **Color-coded priority system** for easy identification
- **Responsive design** that works on all screen sizes

### 🔐 **Authentication**
- **Google Sign-In** integration
- **Firebase Authentication** for secure user management
- **Session persistence** across app restarts
- **User profile management** with avatars

### 🔔 **Smart Notifications**
- **Deadline reminders** with customizable scheduling
- **Health break reminders** for work-life balance
- **Login/logout notifications** for security awareness
- **Local notification support** for all platforms

## 🚀 Getting Started

### Prerequisites

- **Flutter SDK** (3.8.1 or higher)
- **Dart SDK** (3.0.0 or higher)
- **Android Studio** / **VS Code** with Flutter extensions
- **Firebase project** (for backend services)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/remotework_tracker.git
   cd remotework_tracker
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Set up Firebase**
   - Create a new Firebase project
   - Enable Authentication (Google Sign-In)
   - Enable Firestore Database
   - Download and add `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
   - Update Firebase configuration in `lib/firebase_options.dart`

4. **Generate Hive adapters** (for offline support)
   ```bash
   flutter packages pub run build_runner build
   ```

5. **Run the application**
   ```bash
   flutter run
   ```

## 🏗️ Project Structure

```
lib/
├── main.dart                          # App entry point
├── auth_gate.dart                     # Authentication flow
├── auth_service.dart                  # Firebase auth service
├── firebase_options.dart              # Firebase configuration
├── core/
│   ├── constants/                     # App constants
│   ├── services/
│   │   └── local_notification_service.dart
│   └── utils/                         # Utility functions
├── data/
│   ├── local/                         # Local storage
│   ├── models/                        # Data models
│   └── remote/                        # Remote data sources
├── features/
│   ├── analytics/                     # Analytics features
│   ├── calendar/                      # Calendar integration
│   ├── github/                        # GitHub integration
│   ├── tasks/                         # Task management
│   │   ├── add_task_form.dart
│   │   ├── task_controller.dart
│   │   ├── task_model.dart
│   │   ├── task_screen.dart
│   │   └── productivity_dashboard.dart
│   └── timer/                         # Timer features
└── presentation/
    ├── screens/
    │   └── dashboard_screen.dart
    └── widgets/                       # Reusable widgets
```

## 🛠️ Technologies Used

### **Frontend**
- **Flutter** - Cross-platform UI framework
- **Dart** - Programming language
- **Material Design 3** - Design system

### **Backend & Storage**
- **Firebase Authentication** - User authentication
- **Cloud Firestore** - NoSQL database
- **Hive** - Local database for offline support

### **State Management**
- **Flutter Riverpod** - State management solution

### **UI/UX Libraries**
- **fl_chart** - Beautiful charts and graphs
- **BackdropFilter** - Frost glass effects

### **Utilities**
- **connectivity_plus** - Network connectivity monitoring
- **flutter_local_notifications** - Local notifications
- **permission_handler** - Permission management
- **uuid** - Unique ID generation
- **intl** - Internationalization

## 📱 Screenshots

### Main Features
- **Task Management Screen** - Create and manage tasks with priority levels
- **Productivity Dashboard** - Visual statistics and monthly charts
- **Offline Mode** - Work without internet with sync indicators
- **Beautiful UI** - Frost glass effects and modern design

## 🔧 Configuration

### Firebase Setup
1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
2. Enable Authentication with Google Sign-In
3. Enable Firestore Database
4. Download configuration files and add them to the project

### Environment Variables
Create a `.env` file in the root directory:
```env
FIREBASE_PROJECT_ID=your-project-id
GOOGLE_CLIENT_ID=your-google-client-id
```

## 🚀 Deployment

### Android
```bash
flutter build apk --release
```

### iOS
```bash
flutter build ios --release
```

### Web
```bash
flutter build web --release
```

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Flutter Team** for the amazing framework
- **Firebase** for backend services
- **Material Design** for design guidelines
- **Open source community** for various packages

## 📞 Support

If you have any questions or need help, please:
- **Contact the maintainer** at [srinathsaravanan5525@gmail.com]

## 🔄 Changelog

### Version 1.0.0
- ✅ Initial release
- ✅ Task management with priority levels
- ✅ Productivity dashboard with charts
- ✅ Offline support with automatic sync
- ✅ Beautiful frost glass UI
- ✅ Google Sign-In authentication
- ✅ Smart notifications system

---

**Made with ❤️ by [Your Name]**

*Empowering remote workers to stay productive and organized!*
