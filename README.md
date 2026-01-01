🧾 OptiBill:
Offline Billing Application

OptiBill is an offline-first billing application built using Flutter and Hive.
It is designed for small businesses to manage products, generate invoices, and store billing data locally on the device without depending on continuous internet connectivity.
The application also provides backup and restore functionality to prevent data loss.

🚀 Features

📦 Product management (add, edit, view products)

🧮 Invoice creation and billing workflow

🗂️ Offline local data storage using Hive

📄 PDF invoice generation

☁️ Backup and restore using Google Drive

🔐 Offline app lock for access control

⚡ Fast and lightweight offline-first architecture

🛠️ Tech Stack

Frontend

Flutter (Material UI)

Local Database

Hive

Hive Flutter

PDF & Printing

pdf

printing

Backup & Restore

Google Sign-In

Google Drive API

Utilities

intl (date and currency formatting)

uuid (unique identifiers)

connectivity_plus (network availability check)

shared_preferences (local settings storage)

🔄 Data Flow Overview

The user interacts with the Flutter UI

Data is passed to service classes via Dart method calls

Data is stored locally in Hive boxes as binary data using TypeAdapters

The UI reads data directly from Hive and updates instantly

During backup, Hive data is uploaded securely to Google Drive using HTTPS

During restore, the data is downloaded and Hive boxes are repopulated

🔐 App Lock (Offline)

OptiBill includes a simple offline app lock to restrict access to the application on the device.

All data is stored locally on the phone

No server-side authentication is used

The lock functions only as an application-level access control

🔑 Demo App Lock Credentials (For Evaluation)

Username: admin

Password: password123

Recovery Key: buddy

⚠️ These credentials are provided only for demo and evaluation purposes.
In real usage, users can change the app lock password locally.

📂 Project Structure

models – Hive data models and adapters

screens – User interface screens

services – Business logic and data handling

utils – PDF generation and helper utilities

main.dart – Application entry point

▶️ Getting Started

Clone the repository
https://github.com/AswinArun7/OptiBill

Install dependencies
flutter pub get

Run the application
flutter run

📌 Use Case

OptiBill is suitable for:

Small shops and vendors

Offline billing environments

Lightweight inventory and invoice management

Users who prefer local data storage over cloud dependency

🚧 Future Enhancements

Multi-user support

Backend synchronization

Advanced reporting and analytics

Biometric-based app lock

👤 Author

Aswin Arun
B.Tech – Electronics and Communication Engineering
Flutter | Hive | Mobile Application Development
