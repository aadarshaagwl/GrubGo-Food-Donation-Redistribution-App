# 🍽️ GrubGo – Food Donation & Redistribution App

**GrubGo** is a mobile application designed to reduce food wastage by connecting **food donors** with **recipients** in real time. The platform enables **individuals, restaurants, NGOs, and organizations** to donate surplus food, while allowing recipients to request and access available food items.  

This project was developed as part of the **Mobile Application Development (MAD) course** and implements key software development principles, emphasizing **user experience, security, and scalability**.

---

## 🚀 Features and Functionality

### 🔐 User Authentication
- Register and log in using **Email/Password** or **Google Sign-In**.
- **Firebase Authentication** ensures secure login, session management, and password recovery.

### 🍴 Food Donation System
- Donors can list surplus food with details:
  - Food name, quantity, expiration date, and images.
- Donations are stored in the database and available in real time.

### 🥗 Food Receiving System
- Recipients can browse available donations.
- Submit requests based on needs.
- Upon request, **donor contact details** are shared.

### 📍 Location-Based Services
- **Google Maps API** integration to find nearby food donors & NGOs.
- View donor locations on an interactive map.

### 📜 Order History Management
- Track donation and request history.
- Clear records option for better management.

### 👤 User Profile Management
- Update name, email, and contact details.
- Profile details stored securely in **Firebase**.

### 📞 Customer Support & Notifications
- **Click-to-call** functionality for quick assistance.
- **Real-time notifications** for new donations, requests, and updates.

---

## 🔒 Security and Data Management
- **Firebase Authentication** for secure access and verification.  
- **SQLite** for offline storage with synchronization when online.  
- **Data Encryption** for sensitive user information.  

---

## 🏗️ System Architecture

### Frontend (User Interface)
- Built using **Kotlin** in **Android Studio**.
- Follows **Material Design** for a clean UI.
- Components: Activity screens, RecyclerViews, navigation elements.

### Backend (Database & Authentication)
- **Firebase Authentication** – Handles login, registration, sessions.
- **Firebase Firestore** – Stores real-time data (users, donations, requests).
- **SQLite Database** – Offline storage for low-network conditions.

### API Integrations
- **Google Maps API** – Location-based donor/NGO search.
- **Firebase Cloud Messaging (FCM)** – Push notifications.
- **Glide** – Efficient image loading.
- **Retrofit** – For API calls (future enhancements).

---

## ⚙️ Core Functional Modules
- **Authentication Module** – Login, registration, session tracking.
- **Donation Module** – Food donation entries + image uploads.
- **Receiving Module** – Browse & request available food.
- **FoodMap Module** – Map view of nearby food donors.
- **History Module** – Track past donations/requests.
- **Customer Care Module** – Direct support via phone/email.

---

## 🔄 Implementation Details

### Authentication Flow
1. Users log in/register with **Firebase Authentication**.  
2. **Google Sign-In** option available.  
3. User sessions persist across restarts.  

### Database Structure
- **Firebase Firestore** → Stores user data, donation listings, request status.  
- **SQLite Local Storage** → Caches donation records for offline use.  

### Data Flow
1. User logs in/registers.  
2. Donor submits food entry → stored in **Firestore**.  
3. Recipient browses & requests food.  
4. System updates database → marks donation as *Requested*.  
5. Donor details shared + notifications triggered.  

---

## 🛠️ Technology Stack

- **Programming Language:** Kotlin (Android Development)  
- **IDE:** Android Studio  
- **Databases:** Firebase Firestore (Cloud) + SQLite (Local)  
- **APIs & Libraries:**
  - Firebase Authentication
  - Firebase Firestore
  - Firebase Cloud Messaging (Push Notifications)
  - Google Maps API
  - Glide (Image Loading)
  - Retrofit (Future API enhancements)

---

## 📲 Setup and Installation

### Prerequisites
- [Android Studio](https://developer.android.com/studio) installed.  
- A Firebase project with **Firestore** and **Authentication** enabled.  
- Google Maps API Key configured.  

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/aadarshaagwl/grubgo.git
