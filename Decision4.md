# Title: Permissions for Transportation App

## Status: 
Proposed

## Context:
The team must decide on the permissions that the transportation application needs to run on users' devices to provide a good and secure experience. Requesting these permissions is to ensure the proper functioning of the app's features and uphold user privacy. This ADR is outlining the permissions needed by the app.

## Decisions:

- **Location Services:**
  This permission is essential for this transportation application. To enable ride booking, tracking, and navigation, this application requires access to the device location and needs continuous access to the device location while using the app. If the device location access stops while using the app, the app is not going to be able to track and use any other navigational features.

- **Push Notifications:**
  To keep the user informed about ride confirmations, driver updates, and important announcements, this application needs permission to send push notifications to the device. This ensures that users remain notified of every movement.

- **Network Access:**
  This transportation application needs internet access for real-time updates, communication with the server, and payment transactions. For the internet connection, this app needs access to mobile data or Wi-Fi while using this application.

## Consequences:

- **Privacy Concerns:**
  Users may show concerns about granting permissions, especially regarding continuous location tracking. Many users may not want to provide all these permissions to the application, and without these permissions, the app may become useless.

- **Legal and Regulatory Compliance:**
  Any failure to comply with privacy regulations or misuse of user data could lead to legal consequences, potentially damaging the reputation of the transportation company and the transportation app.

- **Negative Impact:**
  Certain permissions can have a negative impact on the performance of devices. If continuously active, it may contribute to increased battery consumption.
