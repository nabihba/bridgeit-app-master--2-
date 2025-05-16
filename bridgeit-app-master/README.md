
# BridgeIT

BridgeIT is a platform designed to connect job seekers from the West Bank with global employers, tackling mass unemployment by providing a job marketplace. This app helps job seekers showcase their profiles and connect with potential employers while offering an easy-to-use platform for employers to find top talent.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [API Integration](#api-integration)
- [Database Integration](#database-integration)
- [Project Structure](#project-structure)
- [Future Plans](#future-plans)
- [Contributing](#contributing)
- [License](#license)

## About

BridgeIT aims to provide global job opportunities for young Palestinians. The platform empowers individuals by giving them the tools, mentorship, and training needed to succeed. Employers can search through jobseeker profiles, review their skills, and contact them directly.

## Features

- **User Profiles**: Users can create detailed profiles showcasing their skills, experience, and professional background.
- **Employer and Jobseeker Roles**: Two user types (Employers and Jobseekers) are supported, with tailored functionality for each.
- **Search and Filters**: Employers can filter jobseekers by various criteria to find the perfect candidate.
- **Chat Functionality**: Employers can directly chat with jobseekers.
- **Responsive UI**: The app is designed to be visually appealing and responsive, ensuring a smooth user experience across devices.
- **Database Integration**: User profiles, jobseeker data, and employer information are stored securely using Appwrite.

## Tech Stack

- **Frontend**: React Native, Expo
- **Backend**: Appwrite (for database and API services)
- **Database**: Appwrite's database for storing jobseeker and employer information
- **Routing**: Expo Router
- **UI Components**: Custom reusable components created with React Native

## Installation

### Prerequisites

Ensure you have the following installed:

- Node.js (LTS version)
- npm or yarn
- Expo CLI

### Steps

1. Clone the repository:

```bash
git clone https://github.com/nabihba/bridgeit.git
cd bridgeit
```

2. Install dependencies:

```bash
npm install
npm install -g expo-cli
npx expo install expo-router react-native-safe-area-context react-native-screens expo-linking expo-constants expo-status-bar
npm install react-native react-native-scripts
```

3. Start the app:

```bash
npx expo start
```

You can run the app on:
- [Development builds](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go)

## Project Structure

```
.
├── assets/                     # Images and static files
├── components/                 # Reusable UI components
│   ├── JobSeekerCard.jsx       # Job seeker profile card
│   ├── EmployerCard.jsx        # Employer profile card
│   ├── FilterBar.jsx           # Filter component for job seekers
│   └── ProfileCard.jsx         # Profile display card
├── pages/                      # Page components
│   ├── index.jsx               # Home page
│   ├── login.jsx               # Login page
│   ├── signup.jsx              # Signup page
│   ├── employerhomepage.jsx    # Employer homepage
│   ├── jobseekerdetailspage.jsx # Job seeker details page
│   ├── jobseekersignup.jsx     # Job seeker sign up page
│   └── jobseekerhome.jsx       # Job seeker homepage
├── services/                   # API and database services
│   └── appwrite.js             # Appwrite service for backend
├── app.json                    # Expo configuration
├── package.json                # Project dependencies and scripts
└── README.md                   # This file
```

## Database Structure

### Jobseeker Collection

```json
{
  "name": "string",
  "profession": "string",
  "experienceYears": "double",
  "funFact": "string",
  "skills": ["string"],
  "location": "string"
}
```

### Employer/Company Collection

```json
{
  "companyName": "string",
  "industry": "string",
  "size": "integer",
  "website": "string",
  "description": "string",
  "contactPerson": "string",
  "location": "string",
  "socialLinks": "string",
  "userId": "string"
}
```

## Future Plans 🔮🚀

We’ve got big dreams for BridgeIT—and we’re just getting started. Here’s what’s on our radar for the next evolution of the platform:

1. **End-to-End Encryption 🔐**  
   Every piece of personal and employment-related data will be protected using advanced end-to-end encryption protocols—think **Signal-level** security, not just your average Gmail vibes. Your privacy, fully locked down.

2. **Blockchain-Based Credential Validation 🧾✨**  
   To eliminate fraud and increase trust, we’ll integrate with platforms like **TrueProfile.io** or **Learning Machine**. This will allow us to **verify academic degrees, certifications, and professional credentials** using secure blockchain technology.

3. **Cross-Border Payroll Integration 💸🌍**  
   We aim to team up with international payroll solutions like **Deel**, **Remote.com**, or **Oyster**. These partnerships will enable **compliant, seamless, and fast payments across borders**, covering everything from tax handling to local legal compliance.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change. Let’s build something impactful together.

## License

[MIT](https://choosealicense.com/licenses/mit/)
