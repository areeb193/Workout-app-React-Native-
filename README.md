# Workout App - React Native

A comprehensive fitness and workout tracking application built with React Native and Expo. This app helps users discover exercises, calculate BMI, track their fitness journey, and maintain a healthy lifestyle.

## 📱 Features
![Fitness Pro](https://res.cloudinary.com/ddz3jxlit/image/upload/v1770025453/Fitness_Pro_1_vatnn3.png)
- **Exercise Database**: Browse exercises by body parts (chest, back, arms, legs, shoulders, etc.)
- **Exercise Details**: View detailed instructions, target muscles, equipment needed, and animated demonstrations
- **BMI Calculator**: Calculate and track your Body Mass Index
- **User Profile**: Manage your personal fitness profile
- **Beautiful UI**: Modern, responsive design with smooth animations
- **Image Carousel**: Motivational fitness images and tips
- **Cross-Platform**: Works on iOS, Android, and Web

## 🎯 What is This Project?

This is a workout and fitness tracking application designed to help users:
- Find exercises targeting specific body parts
- Learn proper exercise techniques with step-by-step instructions
- Monitor their health with the integrated BMI calculator
- Stay motivated with an intuitive and engaging user interface

The app uses the ExerciseDB API to fetch a comprehensive database of exercises with detailed information and visual demonstrations.

## 🚀 How to Get Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v14 or higher) - [Download here](https://nodejs.org/)
- **npm** or **yarn** package manager
- **Expo CLI** (will be installed with dependencies)
- **Git** - [Download here](https://git-scm.com/)

For mobile development:
- **iOS**: macOS with Xcode installed
- **Android**: Android Studio with an emulator configured
- **Physical Device**: Expo Go app installed ([iOS](https://apps.apple.com/app/expo-go/id982107779) | [Android](https://play.google.com/store/apps/details?id=host.exp.exponent))

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/areeb193/Workout-app-React-Native-.git
   cd Workout-app-React-Native-
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```
   or if you prefer yarn:
   ```bash
   yarn install
   ```

3. **Configure API Key** (Optional but Recommended)
   
   The app uses ExerciseDB API for fetching exercises. You can:
   - Use the existing API key in `src/constants/index.js` (included for demo purposes)
   - Or get your own free API key from [RapidAPI - ExerciseDB](https://rapidapi.com/justin-WFnsXH_t6/api/exercisedb)
   
   To use your own API key, update the `rapidApiKey` in `src/constants/index.js`:
   ```javascript
   export const rapidApiKey = 'YOUR_API_KEY_HERE';
   ```

4. **Start the Development Server**
   ```bash
   npm start
   ```
   or
   ```bash
   expo start
   ```

### Running the App

After starting the development server, you have several options:

#### Option 1: Using Expo Go App (Easiest for Beginners)
1. Install Expo Go on your mobile device
2. Scan the QR code displayed in the terminal or browser
3. The app will load on your device

#### Option 2: iOS Simulator (macOS only)
```bash
npm run ios
```

#### Option 3: Android Emulator
```bash
npm run android
```

#### Option 4: Web Browser
```bash
npm run web
```

## 📁 Project Structure

```
Workout-app-React-Native-/
├── api/                      # API integration files
│   └── exerciseDG.js        # ExerciseDB API calls
├── assets/                   # Images, icons, and static resources
│   ├── welcome.png
│   ├── avatar.png
│   ├── slide1.png - slide5.png
│   └── [body part images]
├── src/
│   ├── app/                 # Main application screens (Expo Router)
│   │   ├── index.jsx        # Welcome screen
│   │   ├── home.jsx         # Home screen with body parts
│   │   ├── exercises.jsx    # Exercise list by body part
│   │   ├── exerciseDetails.jsx  # Detailed exercise view
│   │   ├── BmiCalculatorScreen.jsx  # BMI calculator
│   │   ├── ProfileScreen.jsx    # User profile
│   │   ├── about.jsx        # About screen
│   │   └── _layout.jsx      # App layout configuration
│   ├── components/          # Reusable React components
│   │   ├── BodyParts.jsx    # Body parts selection grid
│   │   ├── ExerciseList.jsx # Exercise cards list
│   │   └── ImageSlider.jsx  # Image carousel component
│   ├── constants/           # App constants and configurations
│   │   └── index.js         # API keys, data constants
│   └── context/             # React Context for state management
│       └── ProfileContext.jsx
├── app.json                 # Expo configuration
├── package.json             # Dependencies and scripts
├── babel.config.js          # Babel configuration
├── tailwind.config.js       # Tailwind CSS configuration
└── README.md               # This file

```

## 🛠️ Technologies Used

- **React Native** - Cross-platform mobile development framework
- **Expo** - Development platform for React Native
- **Expo Router** - File-based routing for React Native
- **NativeWind** - Tailwind CSS for React Native
- **Axios** - HTTP client for API requests
- **React Native Reanimated** - Smooth animations
- **React Native Gesture Handler** - Touch gesture handling
- **ExerciseDB API** - Exercise database from RapidAPI

## 🎨 App Screens

1. **Welcome Screen**: Eye-catching landing page with "Get Started" button
2. **Home Screen**: Displays user greeting, profile avatar, BMI calculator access, and body part categories
3. **Exercises Screen**: Shows all exercises for a selected body part
4. **Exercise Details**: Comprehensive exercise information with instructions and animations
5. **BMI Calculator**: Interactive calculator with gender selection, height, and weight inputs
6. **Profile Screen**: User profile management

## 📝 Usage Guide

### For New Users:

1. **Launch the App**: Start the app and tap "Get Started" on the welcome screen
2. **Set Up Profile**: Add your name and personal information
3. **Browse Exercises**: Select a body part to view related exercises
4. **View Exercise Details**: Tap any exercise to see detailed instructions
5. **Calculate BMI**: Use the calculator icon to check your Body Mass Index
6. **Stay Motivated**: Browse the image carousel for fitness tips and motivation

## 🔑 API Configuration

This app uses the ExerciseDB API from RapidAPI. The API provides:
- 1300+ exercises with animations
- Exercise details including target muscles
- Equipment requirements
- Step-by-step instructions

To get your own API key:
1. Visit [RapidAPI ExerciseDB](https://rapidapi.com/justin-WFnsXH_t6/api/exercisedb)
2. Sign up for a free account
3. Subscribe to the free tier
4. Copy your API key
5. Replace the key in `src/constants/index.js`

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this app:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available for educational purposes.

## 👨‍💻 Author

**Areeb**
- GitHub: [@areeb193](https://github.com/areeb193)

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check the [Expo documentation](https://docs.expo.dev/)
- Visit [React Native documentation](https://reactnative.dev/)

## 🙏 Acknowledgments

- ExerciseDB API for providing the comprehensive exercise database
- Expo team for the amazing development platform
- React Native community for continuous support and resources

---

**Happy Working Out! 💪🏋️‍♂️**
