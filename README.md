# 30-Day Flutter Learning Roadmap for Arch + Gnome

## 🚀 Phase 1: Setup & Fundamentals (Days 1-7)

### Day 1-2: Environment Setup

**Install Flutter on Arch:**
```bash
# Install yay if you don't have it
sudo pacman -S --needed git base-devel
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si

# Install Dart
yay -S dart

# Install Android tools
yay -S android-tools

# Install Flutter
yay -S flutter

# Set permissions
sudo groupadd flutterusers
sudo gpasswd -a $USER flutterusers
sudo chown -R :flutterusers /opt/flutter
sudo chmod -R g+w /opt/flutter/

# Add to PATH (add to ~/.bashrc or ~/.zshrc)
export PATH="$PATH:/opt/flutter/bin"
export ANDROID_SDK_ROOT="$HOME/android-sdk"
export PATH="$PATH:$ANDROID_SDK_ROOT/platform-tools"

# Source your shell config
source ~/.bashrc  # or ~/.zshrc

# Check installation
flutter doctor
```

**IDE Setup:**
- Install VS Code: `yay -S visual-studio-code-bin`
- Extensions: Flutter, Dart

**Resources:**
- [Arch Flutter Setup Guide](https://medium.com/@rajgadhiya011/how-to-setup-flutter-on-arch-linux-with-android-sdk-a-step-by-step-guide-f40450b55669)
- [Official Flutter Install](https://docs.flutter.dev/install/manual)

### Day 3-4: Dart Basics

**Learn:**
- Variables, data types, functions
- OOP concepts: classes, inheritance
- Null safety
- Collections (List, Map, Set)
- Async/await

**Resources:**
- [Dart Official Tutorials](https://dart.dev/tutorials)
- YouTube: Flutter official channel's Dart basics
- [DartPad](https://dartpad.dev/) - practice online

### Day 5-7: Flutter Basics

**Learn:**
- Flutter architecture
- Widgets (StatelessWidget, StatefulWidget)
- Basic layouts (Container, Row, Column)
- Material Design basics
- Hot reload concept

**Resources:**
- [Flutter Official Docs](https://flutter.dev/learn)
- [Flutter Codelabs](https://docs.flutter.dev/codelabs)
- YouTube: "Flutter Tutorial for Beginners" by The Net Ninja

---

## 🎨 Phase 2: UI & State Management (Days 8-15)

### Day 8-10: Advanced Widgets

**Learn:**
- ListView, GridView
- Forms and input validation
- Navigation & Routing
- Buttons, Cards, AppBar
- Icons and Images

**Project:** Build a simple Contact List app

**Resources:**
- [Flutter Widget Catalog](https://flutter.dev/docs/development/ui/widgets)
- [Flutter Widget of the Week](https://www.youtube.com/playlist?list=PLjxrf2q8roU23XGwz3Km7sQZFTdB996iG)

### Day 11-13: State Management

**Learn:**
- setState basics
- Provider package
- InheritedWidget
- State lifecycle

**Project:** Todo List App with Provider

**Resources:**
- [Provider Documentation](https://pub.dev/packages/provider)
- YouTube: "Flutter State Management" by Code With Andrea
- [Official State Management Guide](https://flutter.dev/docs/development/data-and-backend/state-mgmt/intro)

### Day 14-15: Navigation & Themes

**Learn:**
- Named routes
- Passing data between screens
- Dark/Light themes
- Custom themes

**Project:** Multi-screen Calculator app

---

## 🔌 Phase 3: Backend & APIs (Days 16-21)

### Day 16-17: HTTP & REST APIs

**Learn:**
- http package
- dio package
- JSON parsing
- Error handling
- API integration

**Project:** Weather App using OpenWeatherMap API

**Resources:**
- [http package](https://pub.dev/packages/http)
- [dio package](https://pub.dev/packages/dio)
- [REST API Tutorial](https://www.freecodecamp.org/news/how-to-develop-a-flutter-app-from-scratch/)

### Day 18-19: Local Storage

**Learn:**
- SharedPreferences
- SQLite (sqflite)
- Hive database
- File storage

**Project:** Note-taking app with local storage

**Resources:**
- [Data persistence guide](https://flutter.dev/docs/cookbook/persistence)
- [sqflite package](https://pub.dev/packages/sqflite)

### Day 20-21: Firebase Basics

**Learn:**
- Firebase setup
- Authentication (Email, Google)
- Firestore basics
- Cloud Storage

**Project:** Simple chat app prototype

**Resources:**
- [FlutterFire Docs](https://firebase.flutter.dev/)
- YouTube: "Flutter & Firebase" by The Net Ninja

---

## 🎯 Phase 4: Advanced & Final Project (Days 22-30)

### Day 22-23: Advanced Concepts

**Learn:**
- Animations
- Custom painters
- Platform-specific code
- Gestures

**Resources:**
- [Flutter Animation Guide](https://flutter.dev/docs/development/ui/animations)
- YouTube: Code With Andrea animations playlist

### Day 24-25: Best Practices

**Learn:**
- Project structure
- Code organization
- Error handling
- Testing basics
- Performance optimization

**Resources:**
- [Flutter Best Practices](https://docs.flutter.dev/perf/best-practices)
- [Effective Dart](https://dart.dev/guides/language/effective-dart)

### Day 26-30: Final Project

**Choose ONE project to build:**

1. **Expense Tracker App**
   - Local storage
   - Charts/graphs
   - Categories
   - Export data

2. **Recipe App**
   - API integration
   - Search functionality
   - Favorites (local storage)
   - Beautiful UI

3. **Fitness Tracker**
   - BMI calculator
   - Workout plans
   - Progress tracking
   - Charts

4. **News Reader App**
   - News API integration
   - Categories
   - Search
   - Bookmarks

**Project Resources:**
- [70+ Flutter Projects](https://www.theinsaneapp.com/2021/06/flutter-projects-with-source-code.html)
- [Flutter Projects GitHub](https://github.com/topics/flutter-projects)
- [30 Project Ideas](https://medium.com/@fyattani/30-flutter-projects-ideas-for-beginners-to-advanced-developers-5731f021f945)

---

## 📚 Essential Free Resources

### Documentation
- [Official Flutter Docs](https://flutter.dev/docs)
- [Dart Language Tour](https://dart.dev/guides/language/language-tour)
- [Flutter Cookbook](https://flutter.dev/docs/cookbook)

### YouTube Channels (Free & Recent)
1. **Flutter** (Official) - Latest updates and widgets
2. **The Net Ninja** - Comprehensive beginner series
3. **Code With Andrea** - Best practices and architecture
4. **Reso Coder** - Clean architecture tutorials
5. **Flutter Mapp** - Weekly tutorials
6. **Marcus Ng** - UI designs

### Practice Platforms
- [DartPad](https://dartpad.dev/) - Online Dart/Flutter editor
- [Flutter Codelabs](https://flutter.dev/codelabs)
- [Exercism - Dart Track](https://exercism.org/tracks/dart)

### Communities
- [Flutter Discord](https://discord.gg/flutter)
- [r/FlutterDev](https://reddit.com/r/FlutterDev)
- [Flutter Slack](https://fluttercommunity.dev/slack)

### GitHub Resources
- [Awesome Flutter](https://github.com/Solido/awesome-flutter) - Curated list
- [Flutter Samples](https://github.com/flutter/samples) - Official samples
- [Flutter Examples](https://github.com/nisrulz/flutter-examples)

---

## 💡 Daily Study Tips

1. **Code Every Day** (2-4 hours minimum)
2. **Build, Don't Just Watch** - Type every line yourself
3. **Debug Your Own Errors** - Google is your friend
4. **Join Discord/Reddit** - Ask questions
5. **Read Official Docs** - Best source of truth
6. **Commit to GitHub** - Track your progress
7. **Don't Get Stuck** - If stuck >30 mins, ask for help

## 🎯 Week-by-Week Goals

**Week 1:** Setup complete, understand Dart, build first Flutter app  
**Week 2:** Master widgets, build 2-3 simple apps  
**Week 3:** APIs and storage, build data-driven app  
**Week 4:** Build impressive final project

---

## ⚡ Quick Commands Reference

```bash
# Create new project
flutter create my_app

# Run app
flutter run

# Check for issues
flutter doctor

# Hot reload
r (in terminal while app running)

# Hot restart
R

# Clean build
flutter clean && flutter pub get

# Install packages
flutter pub add package_name

# Update Flutter
flutter upgrade
```

---

## 🔥 Success Checklist

- [ ] Flutter installed and `flutter doctor` shows no errors
- [ ] Built "Hello World" app
- [ ] Understand StatelessWidget vs StatefulWidget
- [ ] Built a UI with 5+ different widgets
- [ ] Implemented navigation between screens
- [ ] Used Provider for state management
- [ ] Integrated at least one REST API
- [ ] Stored data locally
- [ ] Completed one full project with 3+ screens
- [ ] Code pushed to GitHub

---

**Remember:** 30 days is tight but doable! Focus on building rather than perfection. Good luck! 🚀
