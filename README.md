# Internet Whiteboard Application 
Internet Whiteboard Application is an Internet-based collaborative whiteboard application developed to enhance communication and collaboration for remote consulting services. This application allows users to create whiteboard sessions where participants can draw, type text, and use various shape drawing tools in real-time. The system provides a secure and encrypted environment for all user interactions.

## Key Features
### User Account Management:
- Create and manage admin, employee, and customer accounts.
- Account validation period and login details sent via email.
- User account data stored in a secure SQL database.
### Whiteboard Session Functionality:
- Real-time whiteboard sheets for simultaneous drawing and text typing.
- Standard shape drawing tools (line, arrow, circle, oval, square, rectangle, poly-line, text, eraser, and free-drawing tool).
- Customization options for tools, including thickness, color, and filling color for shapes, and font, size, italics, and bold for text.
- Designation of a moderator for each session with lock, undo, and sheet change capabilities.
### Modification and Undo Operations:
- All modifications saved in a list on the admin server.
- Modification data includes index, timestamp, user name, modification type, and affected sheet.
- Sequential undo operations by the moderator.
- Distinct and non-modifiable undo modifications.
### Data Persistence and Playback:
- Save and reload the list of changes for whiteboard sessions.
- Clear whiteboard upon reloading.
- Sequential navigation of modifications with user name and timestamp display.
- Automatic playback of modifications with adjustable delay.
### Security and Encryption:
- SSL/TLS certificates for encrypted user-to-user and user-to-server communication.
- Self-signed certificates for initial release to customers.
- Support for disabling encryption for debugging purposes.

## Technology Stack
### Backend:
- Python with Flask/Django for server-side development.
- PostgreSQL for user account and modification data storage.
- OpenSSL/LibreSSL for SSL/TLS support.
### Frontend:
- HTML5, CSS3, and JavaScript for client-side development.
- JavaScript library (e.g., Fabric.js) for whiteboard functionalities.