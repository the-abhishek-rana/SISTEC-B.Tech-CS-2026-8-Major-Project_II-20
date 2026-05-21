# Unified Mobile System for Managing Esports Tournaments and Events

<div align="center">

![Version](https://img.shields.io/badge/Version-1.0-blue)
![License](https://img.shields.io/badge/License-Academic-green)
![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)
![Language](https://img.shields.io/badge/Language-Kotlin-purple)

A comprehensive mobile application designed to streamline the organization, execution, and participation in esports competitions.

[About](#about) • [Features](#features) • [Tech Stack](#tech-stack) • [Installation](#installation) • [Usage](#usage) • [Project Structure](#project-structure)

</div>

---

## About

The **Unified Mobile System for Managing Esports Tournaments and Events** is a comprehensive digital platform developed for B.Tech Major Project II at Sagar Institute of Science & Technology (SISTec), Bhopal. This Android-based application addresses the challenges of fragmented tournament management tools by providing an integrated solution for organizing, managing, and participating in esports competitions.

### Motivation

The rapid expansion of the esports industry has created a critical need for efficient tournament management solutions. Traditional methods rely on fragmented tools (spreadsheets, messaging apps, standalone platforms), leading to:
- Scheduling conflicts and data inconsistencies
- Manual, error-prone processes
- Poor coordination between stakeholders
- Limited mobile optimization
- Lack of centralized management

This project aims to solve these challenges by providing a unified, scalable, and secure platform accessible via mobile devices.

### Alignment with UN SDGs

This project supports:
- **SDG 8**: Decent Work and Economic Growth
- **SDG 9**: Industry, Innovation and Infrastructure
- **SDG 17**: Partnerships for the Goals

---

## Features

### 🎮 Core Features

#### Tournament Management
- **Create & Manage Tournaments**: Organizers can create tournaments with custom configurations
- **Automated Bracket Generation**: Automatic tournament bracket creation and management
- **Match Scheduling**: Intelligent match scheduling with conflict prevention
- **Real-Time Updates**: Live match tracking and result updates

#### User Management
- **Registration & Authentication**: Secure user registration and login
- **Role-Based Access**: Different dashboards for admins, players, and spectators
- **Profile Management**: User profile creation and management
- **Team Management**: Create and manage gaming teams

#### Communication & Notifications
- **Push Notifications**: Instant notifications for match timings, results, and updates
- **Chat & Messaging**: In-app communication between players and organizers
- **Announcements**: Real-time announcement broadcasting

#### Match & Streaming
- **Live Match Updates**: Real-time match score and status updates
- **Leaderboards & Rankings**: Dynamic player and team rankings
- **Live Streaming Integration**: Built-in streaming capabilities
- **Match Results**: Comprehensive match result tracking

#### Analytics & Payments
- **Performance Analytics**: Player statistics and performance metrics
- **Payment Processing**: Secure entry fee management
- **Event Analytics**: Detailed tournament analytics and reports
- **Wallet System**: In-app wallet for prize distribution

### 🤖 Machine Learning Module

The ML Module enhances platform intelligence with:
- **Player Skill Prediction**: Analyzes gameplay statistics to determine skill levels (Beginner, Intermediate, Professional, Elite)
- **Smart Matchmaking**: Creates balanced matches using skill ratings, region, ping, and performance
- **Tournament Recommendations**: Suggests suitable tournaments based on player interests and history
- **Fraud Detection**: Identifies suspicious activities, cheating, smurfing, and account abuse using anomaly detection

---

## Tech Stack

### Frontend
- **Language**: Kotlin 1.96
- **IDE**: Android Studio
- **Framework**: Android SDK (API 24+)
- **UI Components**: Jetpack Compose, Material Design
- **Build Tool**: Gradle

### Backend & Database
- **Cloud Platform**: Firebase
- **Database**: Firebase Firestore
- **Authentication**: Firebase Authentication
- **Real-time Database**: Firebase Realtime Database
- **Messaging**: Firebase Cloud Messaging (FCM)

### Development Tools
- **Version Control**: Git
- **Development OS**: Windows 10/11, macOS, or Linux
- **Code Editor**: VS Code 1.9.x

### Architecture
- **Design Pattern**: MVC (Model-View-Controller)
- **Architecture**: 1-Tier Client-Server with Cloud Backend
- **Methodology**: Agile SDLC Model

---

## Requirements

### Hardware Requirements

#### Development Machine
| Component | Specification |
|-----------|---------------|
| Processor | Intel i5 / Ryzen 5 or higher |
| RAM | Minimum 8 GB (16 GB recommended) |
| Storage | SSD 256 GB or more |
| Graphics | Integrated GPU |

#### Testing Device
| Requirement | Specification |
|-----------|---------------|
| OS | Android 8.0+ |
| RAM | Minimum 4 GB |
| Processor | Modern processor |
| Screen Size | 4.5" - 6.5" |

#### Alternative (iOS)
| Requirement | Specification |
|-----------|---------------|
| Device | iPhone 8 or later |
| OS | iOS 12 or later |

### Software Requirements

| Software | Version |
|----------|---------|
| Android Studio | Latest LTS |
| Android SDK | API Level 24+ |
| JDK | 11 or higher |
| Gradle | 7.0+ |
| Kotlin | 1.96+ |
| Firebase SDK | 33.x.x |

### Internet Requirements
- Stable 4G/5G or Wi-Fi connection
- Minimum bandwidth: 2 Mbps (for basic usage)
- Minimum bandwidth: 5 Mbps (for live streaming)

---

## Installation

### Prerequisites
Before you begin, ensure you have installed:
- Android Studio (Latest version)
- JDK 11 or higher
- Git
- Firebase account (with a new project created)

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/esports-tournament-manager.git
cd esports-tournament-manager
```

### Step 2: Set Up Firebase
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new Firebase project
3. Enable the following services:
   - Authentication (Email/Password, Google Sign-In)
   - Firestore Database
   - Realtime Database
   - Cloud Messaging (FCM)
   - Storage

4. Download `google-services.json` from Firebase Console
5. Place it in: `app/google-services.json`

### Step 3: Configure Firebase Credentials
```bash
# Copy the Firebase configuration file
cp google-services.json app/
```

### Step 4: Open in Android Studio
```bash
1. Open Android Studio
2. File → Open → Select project directory
3. Wait for Gradle sync to complete
```

### Step 5: Update Dependencies
```bash
# In Android Studio terminal
./gradlew build
```

### Step 6: Build and Run
```bash
# Build APK
./gradlew assembleDebug

# Install on connected device/emulator
./gradlew installDebug

# Or directly run on device
./gradlew run
```

### Step 7: Configure Android Emulator (Optional)
If you don't have a physical device:
```bash
# Create emulator using Android Studio AVD Manager
# Or use command line:
emulator -avd YourEmulatorName
```

---

## Usage

### For Tournament Organizers (Admin)

1. **Register & Login**
   - Create an account with email/password
   - Login to Admin Dashboard

2. **Create Tournament**
   - Navigate to "Create Tournament"
   - Enter tournament details (name, game, prize pool, entry fee)
   - Configure tournament settings
   - Publish tournament

3. **Manage Tournaments**
   - View all tournaments
   - Edit tournament details
   - Delete tournaments
   - Monitor registrations

4. **Schedule Matches**
   - Automatically generate brackets
   - Schedule match timings
   - Assign teams/players to matches

5. **Send Notifications**
   - Notify players about match updates
   - Send announcements
   - Broadcast match results

### For Players

1. **Register & Login**
   - Create player account
   - Setup gaming profile
   - Add game preferences

2. **Join Tournament**
   - Browse available tournaments
   - View tournament details
   - Register for tournaments
   - Pay entry fee (if required)

3. **Track Matches**
   - View upcoming matches
   - Track match schedules
   - View live scores
   - Check results

4. **View Leaderboard**
   - Check player rankings
   - View statistics
   - Track progress

### For Spectators

1. **Browse Tournaments**
   - View live tournaments
   - Check tournament details

2. **Watch Live Streams**
   - Access live streaming
   - View live scores
   - Follow match updates

3. **View Leaderboards**
   - Check player rankings
   - View match statistics
   - Follow player performance

---

## Project Structure

```
esports-tournament-manager/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/thethirdeye/
│   │   │   │   ├── admin/
│   │   │   │   │   ├── AdminMainActivity.kt
│   │   │   │   │   ├── AdminTournamentFragment.kt
│   │   │   │   │   ├── AllTournamentActivity.kt
│   │   │   │   │   └── CreateTournamentActivity.kt
│   │   │   │   ├── auth/
│   │   │   │   │   ├── LoginActivity.kt
│   │   │   │   │   └── RegisterActivity.kt
│   │   │   │   ├── main/
│   │   │   │   │   └── MainActivity.kt
│   │   │   │   ├── model/
│   │   │   │   │   ├── TournamentModel.kt
│   │   │   │   │   ├── PlayerModel.kt
│   │   │   │   │   └── MatchModel.kt
│   │   │   │   ├── adapter/
│   │   │   │   │   └── TournamentAdapter.kt
│   │   │   │   └── util/
│   │   │   │       └── Constants.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   ├── values/
│   │   │   │   └── drawable/
│   │   │   └── AndroidManifest.xml
│   │   └── test/ & androidTest/
│   └── build.gradle
│
├── gradle/
├── build.gradle (Project level)
├── settings.gradle
├── google-services.json
├── README.md
└── LICENSE
```

### Key Directories Explained

| Directory | Purpose |
|-----------|---------|
| `admin/` | Admin-specific activities and fragments |
| `auth/` | Authentication activities (Login, Register) |
| `main/` | Main player activities |
| `model/` | Data models (Tournament, Player, Match) |
| `adapter/` | RecyclerView adapters |
| `util/` | Utility classes and constants |
| `res/` | Resources (layouts, strings, drawables) |

---

## Database Schema

### Firestore Collections

#### Users Collection
```json
{
  "user_id": "INT",
  "username": "VARCHAR",
  "email": "VARCHAR",
  "password": "VARCHAR (Hashed)",
  "role": "VARCHAR (admin/player/spectator)",
  "phone": "VARCHAR"
}
```

#### Tournaments Collection
```json
{
  "tournament_id": "INT",
  "title": "VARCHAR",
  "game_name": "VARCHAR",
  "start_date": "DATE",
  "end_date": "DATE",
  "prize_pool": "DECIMAL",
  "status": "VARCHAR"
}
```

#### Players Collection
```json
{
  "player_id": "INT",
  "gamer_tag": "VARCHAR",
  "rank": "VARCHAR",
  "user_id": "INT",
  "skill_level": "VARCHAR"
}
```

#### Matches Collection
```json
{
  "match_id": "INT",
  "match_date": "DATE",
  "result": "VARCHAR",
  "tournament_id": "INT"
}
```

---

## API Integration

### Firebase Authentication
```kotlin
val auth = FirebaseAuth.getInstance()
auth.signInWithEmailAndPassword(email, password)
    .addOnSuccessListener { result ->
        // Login successful
    }
    .addOnFailureListener { exception ->
        // Handle error
    }
```

### Firestore Database Operations
```kotlin
val db = FirebaseFirestore.getInstance()

// Create
db.collection("tournaments").add(tournament)

// Read
db.collection("tournaments").get()

// Update
db.collection("tournaments").document(id).update(data)

// Delete
db.collection("tournaments").document(id).delete()
```

---

## Key Features Implementation

### Smart Matchmaking Algorithm
The system uses machine learning to:
- Analyze player win/loss ratios
- Consider kill/death ratios
- Factor in average scores
- Use skill ratings for balanced pairing

### Tournament Recommendation System
- Collaborative filtering based on user preferences
- Content-based filtering on game preferences
- Personalized suggestions based on skill level

### Fraud Detection System
- Anomaly detection algorithms
- Account behavior monitoring
- Suspicious pattern identification
- Real-time alert generation

---

## Testing

### Manual Testing Performed
- User registration and authentication
- Tournament creation and management
- Match scheduling and updates
- Notification delivery
- Payment processing
- UI/UX functionality

### Test Cases Covered
1. Admin creation of tournaments
2. Player registration for tournaments
3. Match scheduling
4. Live score updates
5. Notification delivery
6. Payment transactions
7. Leaderboard updates

### To Run Tests
```bash
# Unit tests
./gradlew test

# Instrumented tests
./gradlew connectedAndroidTest
```

---

## Future Enhancements

### Planned Features
- [ ] AI-based match scheduling with automatic bracket generation
- [ ] Live streaming integration (YouTube, Twitch)
- [ ] Advanced analytics dashboard
- [ ] In-app voice and chat system
- [ ] Mobile app for iOS (currently Android only)
- [ ] Web dashboard for administrators
- [ ] Social features (friend list, teams)
- [ ] Anti-cheat detection system
- [ ] Sponsorship management module
- [ ] Prize distribution automation

### Technology Upgrades
- Integration with Kubernetes for scaling
- Machine learning model improvements
- Real-time data processing with Apache Kafka
- Enhanced security with blockchain verification

---

## Team

**Project Team: Group 20**

| Name | Roll Number | Role |
|------|------------|------|
| Aaryan Chandel | 0188CS221002 | UI/UX Design |
| Abhishek kr Singh | 0188CS221016 | Research & Documentation |
| Ayush Mishra | 0188CS221069 | Backend Development |
| Ravi Shankar kr | 0188CS221165 | Frontend Development |

**Project Guide**: Prof. Pankaj Savita (Assistant Professor)

**Department**: Computer Science & Engineering

**Institution**: Sagar Institute of Science & Technology (SISTec), Bhopal (M.P.)

---

## Development Guidelines

### Code Style
- Follow Kotlin official coding conventions
- Use meaningful variable and function names
- Write comments for complex logic
- Maximum line length: 100 characters

### Naming Conventions
- Classes: PascalCase (e.g., `AdminMainActivity`)
- Functions/Variables: camelCase (e.g., `loadTournaments()`)
- Constants: UPPER_SNAKE_CASE (e.g., `DATABASE_URL`)
- Resources: lowercase_with_underscores (e.g., `activity_main.xml`)

### Git Workflow
```bash
# Create feature branch
git checkout -b feature/feature-name

# Make changes and commit
git add .
git commit -m "Add feature description"

# Push to repository
git push origin feature/feature-name

# Create Pull Request
```

---

## Troubleshooting

### Common Issues & Solutions

**Issue**: Firebase dependency conflicts
```
Solution: Update all Firebase libraries to the same version
./gradlew clean build --stacktrace
```

**Issue**: Gradle sync fails
```
Solution: 
1. File → Invalidate Caches
2. Close project and reopen
3. ./gradlew clean
```

**Issue**: APK installation fails
```
Solution: Ensure minimum Android API is 24
Check build.gradle for minSdkVersion = 24
```

**Issue**: Firebase authentication not working
```
Solution: 
1. Verify google-services.json is in app/ directory
2. Check Firebase project settings
3. Ensure authentication is enabled in Firebase Console
```

---

## Performance Optimization

### Best Practices
- Use RecyclerView for list data
- Implement pagination for large datasets
- Optimize images before adding to resources
- Use lazy loading for database queries
- Implement caching strategies

### Benchmarks
- App startup time: < 3 seconds
- List loading: < 1 second for 100 items
- Match update latency: < 500ms
- Notification delivery: < 2 seconds

---

## Security Features

- **Authentication**: Firebase Email/Password and Google Sign-In
- **Data Encryption**: All sensitive data encrypted in transit (SSL/TLS)
- **Access Control**: Role-based access control (Admin, Player, Spectator)
- **Input Validation**: All user inputs validated before processing
- **Session Management**: Secure session handling with Firebase

### Security Best Practices
1. Never commit `google-services.json` with real credentials
2. Use environment variables for sensitive data
3. Regularly update dependencies
4. Implement proper error handling without exposing sensitive info
5. Use ProGuard for code obfuscation

---

## Literature Survey References

### Research Papers
1. J. Gisbert-Pérez et al., "Key Structure and Processes in Esports Teams: A Systematic Review," *Current Psychology*, 2024.
2. W. Chiu et al., "Knowledge Mapping and Sustainable Development of Esports Research," *Sustainability (MDPI)*, 2021.
3. C. Steinkuehler, "Esports Research: Critical, Empirical, and Historical Studies," *Games and Culture (SAGE)*, 2019.
4. N. Ajah et al., "Esports as a New Economic Frontier: Bibliometric Exploration," *Journal of Technology Management and Technopreneur ship*, 2025.

### Books
5. T. Scholz, *eSports is Business: Management in the World of Competitive Gaming*. Springer, 2019.
6. K. Karhulahti, *Esports and the Global Gaming Industry*. Routledge, 2020.

### Websites
7. [International Esports Federation](https://www.ie-sf.org)
8. [Esports Insider](https://esportsinsider.com)
9. [Liquipedia](https://liquipedia.net)

---

## License

This project is developed as an academic project at Sagar Institute of Science & Technology (SISTec), Bhopal. It is intended for educational purposes.

**Approved by**: AICTE, New Delhi & Govt. of Madhya Pradesh

**Affiliated to**: Rajiv Gandhi Proudyogiki Vishwavidyalaya, Bhopal (M.P.)

---

## Support & Contributions

### Getting Help
- Check existing issues on GitHub
- Create a new issue with detailed description
- Contact project team through institutional email

### Contributing
We welcome contributions! Please:
1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## Contact

**For queries regarding this project, contact:**

- **Project Guide**: Prof. Pankaj Savita
  - Email: pankaj.savita@sistec.ac.in
  
- **Department**: Computer Science & Engineering
  - Email: cse@sistec.ac.in

- **Institution**: Sagar Institute of Science & Technology
  - Address: Gandhi Nagar, Bhopal (M.P.), India
  - Phone: [Institutional Contact]

---

## Acknowledgments

We extend our sincere gratitude to:
- Prof. Pankaj Savita (Project Guide)
- Prof. Deepti Jain (Project Coordinator)
- Prof. Nargish Gupta (HOD, CSE)
- Dr. Swati Saxena (Vice Principal)
- Dr. Manish Billore (Principal)
- All faculty and staff of SISTec for their support and guidance

---

<div align="center">

**Made with ❤️ by Group 20 - SISTec Bhopal**

![GitHub](https://img.shields.io/badge/-GitHub-black?logo=github)
![Firebase](https://img.shields.io/badge/-Firebase-yellow?logo=firebase)
![Android](https://img.shields.io/badge/-Android-green?logo=android)

*Last Updated: June 2026*

</div>
