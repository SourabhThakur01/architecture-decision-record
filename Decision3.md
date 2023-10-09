# Title: Selection of Backend Language for Mobile Transportation App

## Status: 
Proposed

## Context:
The current decision is related to the choice of the backend programming language, which will play a significant role in managing user authentication, coordinating real-time updates, handling data, and ensuring the overall functionality and security of the application.

## Decision:
After considering the project requirements, the team proposes to use **Node.js** as the backend programming language. Node.js is chosen for its event-driven architecture, which aligns well with the real-time nature of the location tracking and messaging features required by the app. Node.js has been chosen for various reasons, including:

- **Real-time Updates and WebSocket Integration:** Node.js' asynchronous nature supports continuous updates, tracking driver and passenger locations, a major requirement of the app. Because this app needs to track both driver and passengers' location and provide updates on their devices, Node.js provides all these functionalities.

- **Authentication and Authorization:** Node.js supports various authentication mechanisms, allowing the team to implement secure methods like email/password, social login, or two-factor authentication. Authorization rules can be efficiently enforced through middleware functions in Node.js.

- **Geolocation Services Integration:** Node.js allows smooth integration with popular geolocation service providers like Google Maps, and the asynchronous feature of Node.js can enhance the responsiveness of geolocation services in the application, a main requirement for this transportation app.

## Consequences:
- **Callback:** Asynchronous programming in Node.js heavily relies on callbacks, which can create problems because managing multiple nested callbacks can make code more difficult to read, maintain, and debug. While solutions like Promises and async/await are available to mitigate these issues, inexperienced developers may find it challenging to deal with callback-related complexities.
