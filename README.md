# Contact Tracing Mobile Application

## Project Explanation
The objective of this comprehensive workshop is to construct a robust contact tracing mobile application from the ground up. The system utilizes Flutter as the primary framework for crafting the mobile app, implementing features such as UDID integration, QR code functionality, positive test reporting, and contact tracing using Bluetooth for proximity tracking. The backend, built with Laravel, includes APIs for data transmission, data processing, and alert generation. Firebase Cloud Messaging (FCM) is integrated for push notifications.

## Features
- **Privacy-preserving**: The architecture maintains privacy by avoiding user registration while utilizing UDID for device identification.
- **Accurate**: Implementing algorithms to process contact logs, detect positive cases, and generate alerts for potentially exposed users ensures accuracy.
- **User-friendly**: The application provides a user-friendly interface with features like onboarding, nearby device tracking, exposure notifications, and positive test reporting.


## Screenshots
Here are some screenshots of the user interface of the mobile application:
1. **Onboarding screen**: Allows the user to create an account by entering their full name, contact number, and occupation in the university (optional).
   ![Onboard Screen](/assets/screenshots/onboard.png)
2. **Home Screen & Nearby Devices Screen**: Shows the user’s current location on a map, as well as the number of nearby devices within a 10-meter radius.
   ![Home Screen](/assets/screenshots/tracing.png)
3. **Exposure Notification Screen**: Shows a message that informs the user that they have been in contact with a confirmed case of COVID-19 within the past 14 days, as well as the date and time of contact.
   ![Exposure notification Screen](/assets/screenshots/alert.png)

## Installation
To install and run the mobile application, follow these steps:
1. Clone this repository to your local machine using `git clone https://github.com/pitiky0/Application-de-Tra-age-de-Contacts`.
2. Install Flutter and Android Studio on your machine.
3. Open the project folder in Android Studio and run `flutter pub get` to install the dependencies.
4. Connect your Android device or emulator to your machine and run `flutter run` to launch the application.

## Usage
To use the mobile application, follow these steps:
1. Register your device by entering your full name, contact number, and occupation in the university (optional).
2. Grant permission for the application to access your Bluetooth.
3. Tap on the "Start Tracing" button to begin collecting and sending your Bluetooth connexion to the server every two minutes.
4. Check the "Nearby Devices" section to see if there are any devices in close proximity to you within a 10-meter radius.
5. If you test positive for COVID-19, report your status through the app by entering the date of your PCR test report.
6. If you receive an exposure notification from the app, follow the instructions to self-quarantine or get tested.

## License
This project is licensed under the MIT License - see the [LICENSE](/LICENSE) file for details.
