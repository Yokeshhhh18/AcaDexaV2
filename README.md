# AcaDexa - Smart Scheduling Platform

<div align="center">
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen" alt="Status" />
  <img src="https://img.shields.io/badge/License-MIT-blue" alt="License" />
  <img src="https://img.shields.io/badge/Technology-Firebase_&_Tailwind-orange" alt="Technology" />
</div>

**AcaDexa** is a modern, single-page web application designed to simplify the complex task of academic scheduling. It provides an intuitive, drag-and-drop interface for managing timetables, coupled with AI-powered features for optimization and conflict resolution. The platform is built with role-based access control, ensuring that administrators have full control while teachers can view their schedules and interact with system notifications.

---

###  Live Demo

**(Link to your deployed website on Vercel or Firebase Hosting)**

---

## ✨ Core Features

* **Interactive Timetable**: Drag-and-drop classes from an "Unscheduled" list directly onto the calendar.
* **Role-Based Access Control**:
    * **Admin (`KASHY`)**: Full access to create, manage, optimize, and approve the schedule. Can view the dashboard and mark teachers absent.
    * **Teacher (`ZAP`)**: View-only access to the schedule. Receives real-time notifications for substitution requests.
* **Approval Workflow**: Admins can submit the schedule for approval, which **locks** it from further edits by non-admins until the admin unlocks it.
* **Real-time Notification System**:
    * Admins receive notifications when a schedule is submitted for approval.
    * Admins receive alerts when a teacher is marked absent.
    * Teachers can receive notifications for substitution requests (future feature).
* **Analytics Dashboard**: Admins can view a dashboard with key metrics, including faculty workload distribution and room capacity utilization charts.
* **AI-Powered Assistance**:
    * **Conflict Detection**: Automatically highlights scheduling conflicts (e.g., double-booked teacher or room).
    * **Schedule Optimizer**: A one-click tool to suggest a more optimal schedule arrangement.
* **Modern UI/UX**:
    * Responsive design for desktop and mobile.
    * Aesthetic theme with a functional Dark Mode.
    * Interactive modals for viewing details and taking actions.
* **AI Chatbot**: An integrated chatbot ("KASHY") to answer questions about the schedule. *(Note: Requires a Google Gemini API Key to be functional).*

---

## 🛠️ Technologies Used

* **Frontend**: HTML5, JavaScript (ES6 Modules)
* **Styling**: Tailwind CSS
* **Backend & Database**: Google Firebase (Firestore for real-time data, Firebase Authentication)
* **Libraries**:
    * [FullCalendar.js](https://fullcalendar.io/): For the interactive timetable.
    * [Chart.js](https://www.chartjs.org/): For the analytics dashboard charts.
    * [Font Awesome](https://fontawesome.com/): For icons.

---

## 🚀 Setup and Installation

To run this project locally, you will need Node.js and a Firebase project.

### 1. Firebase Setup

1.  Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2.  In your project, go to **Project Settings** > **General**. Under "Your apps", click the web icon (`</>`) to create a new web app.
3.  Copy the `firebaseConfig` object. You will need this for the next step.
4.  In the Firebase console, navigate to **Firestore Database** and create a database in **Test mode** to allow reads and writes.

### 2. Local Environment Setup

1.  Clone this repository or download the `index.html` and `package.json` files.
2.  **
