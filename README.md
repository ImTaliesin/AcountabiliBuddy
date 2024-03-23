# AcountabiliBuddy
A desktop app to help you stay accountable


# Setup
npm install typescript --save-dev
npm install electron electron-builder --save-dev
npm install @types/electron --save-dev

# ToDo
Remember to handle edge cases, such as when the user has multiple social media websites open simultaneously or when the app is closed unexpectedly.

Implement website detection:
Use Electron's webContents module to monitor the user's browsing activity.
Detect when the user navigates to a social media website by comparing the URL with a predefined list of social media domains.

Implement timer functionality:
Create a timer class in TypeScript to track the time spent on social media websites.
Start the timer when the user navigates to a social media website and stop it when they navigate away. Do not stray from this idea, the user must not have it open, even it if out of focus it still counts towards the timer. Research suggests even having social media open is a big hit to productivity.
Display the elapsed time in the user interface.

Implement website blocking:
Create a blocking mechanism that prevents the user from accessing social media websites once the time limit is reached.
Use Electron's webContents module to intercept and block requests to social media websites.
Display a notification or overlay to inform the user that they have reached the time limit.

Implement notifications and reminders:
Use Electron's Notification module to display desktop notifications when the user approaches or reaches the time limit.
Optionally, implement reminder notifications to encourage the user to take breaks or limit their social media usage.

Implement user settings:
Allow the user to customize the time limit for social media usage.
Store the user's preferences using Electron's localStorage or a configuration file.
Provide an interface for the user to modify the settings.

Testing and debugging:
Write unit tests for critical components of the app using Jest or Mocha.
Test the app's functionality manually by running it in development mode and verifying the behavior.
Debug any issues that arise during testing and fix them accordingly.

Packaging and distribution:
Use Electron Builder to package your app into a distributable format (e.g., an installer or executable).
Configure the build settings, icons, and metadata for your app.
Generate the packaged app and distribute it to users.
