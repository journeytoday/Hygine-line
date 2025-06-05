# Lightweight Music Equipment Cleaning Reminder App

This application helps musicians and audio professionals keep track of their equipment cleaning schedules. It allows users to add their instruments/equipment, set custom cleaning reminder intervals, and log cleaning events. The app is designed to be lightweight, power-efficient, and respectful of user privacy, with all data stored locally by default and optional cloud sync.

## Core Functional Requirements

### Task Management
- Add, edit, and delete musical instruments or equipment.
- Set custom reminder intervals for each item (e.g., every 7 days).
- Mark tasks as completed with a dedicated button for each instrument.
- Log each completion event with a timestamp.

### Reminders
- Receive reminders only at user-defined intervals per item.
- Reminders utilize Android notification channels (configurable for silent or sound-based alerts).
- Optimized for minimal background activity, running only when reminders are due.

### Data Logging
- Maintain an indefinite log of all cleaning activities.
- Log entries include instrument name, date/time cleaned, and optional notes or photos.
- View, filter, and sort cleaning history within the app.

### Data Export
- Export cleaning logs in CSV format.
- Optionally generate summary reports (e.g., weekly/monthly cleaning history).
- Data export functionality is available entirely offline.

## Storage and Sync

### Local Storage
- All user data, including the equipment list, reminder intervals, cleaning logs, and photos, is stored locally on the device by default.
- Data is retained indefinitely unless explicitly deleted by the user.

### Optional Cloud Sync
- Users have the option to enable cloud sync/backup (e.g., using Google Drive or a simple cloud database).
- The app remains fully functional offline, even if cloud features are not used.

## User Interface

### GUI Design
- The app features a graphical user interface with a minimalist and classy aesthetic.
- It offers a clean layout with intuitive access to:
    - Task list
    - Completion button
    - Reminder settings
    - History log
    - Export options

### User Input
- Users can perform the following actions:
    - Add and edit instrument details (name, category, optional photo).
    - Set custom reminder intervals for each item.
    - View and edit past task logs.
    - Export data via a simple menu or button.

## Performance and Power Use

### Power Optimization
- The app is designed to be power-efficient and performs no background processing unless a reminder is scheduled.
- It avoids the use of wake locks, polling, or frequent wakeups to conserve battery life.
- All reminders and tasks utilize battery-friendly scheduling mechanisms.

## Privacy and Data Handling

### Sensitive Data
- Users may optionally provide basic demographic information and photos of their instruments.
- No encryption or anonymization is applied to user data.
- User data is stored in plain format and kept privately on the device, unless the user opts for manual cloud synchronization.

## Architecture and Maintainability

### Modular Codebase
- The app is structured to support modular updates, allowing for easier addition of new features such as export formats, themes, or statistical analysis.
- It is built to be stable and self-contained, aiming for low-maintenance overhead.
- The codebase is designed for single-developer maintenance, emphasizing clean and well-commented code.

## Compatibility

-   **Minimum Android Version:** 8.0 (API 26)
-   **Key Libraries:**
    -   Built with modern and stable Android libraries.
    -   Utilizes Room for the local database.
    -   Employs WorkManager for scheduling reminders.

## Deployment and Distribution

-   The app will be distributed privately, via APK file or by sideloading.
-   There are no plans for publishing on the Google Play Store.
-   The app does not integrate with Google billing, ads, or compliance APIs.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

What things you need to install the software and how to install them.

### Installing

A step by step series of examples that tell you how to get a development env running.

## Running the tests

Explain how to run the automated tests for this system.

### Break down into end to end tests

Explain what these tests test and why.

## Built With

* Android SDK
* Room Persistence Library
* WorkManager

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

* Hat tip to anyone whose code was used.
* Inspiration
* etc
