Web application for a plumbing company to generate proposals and invoices 


Claud 3.5 says it has the following requirements...

But with those requirements you'll get this:
<img width="1025" alt="Screenshot 2025-03-02 at 11 27 13 PM" src="https://github.com/user-attachments/assets/a370c506-5836-4357-9b6a-811fd0b7028b" />

While I built this:
![screencapture-127-0-0-1-5004-2025-03-02-23_41_02](https://github.com/user-attachments/assets/495aa053-d141-4045-a1ac-07ea9a49eb1a)


Core Features:
1. Flask backend with a modern JavaScript frontend (no framework required)
2. Two main document types: Proposals and Invoices
3. Payment processing integration with QR code generation
4. Voice input capability for content dictation
5. PDF generation functionality

Key Components:

Frontend:
- Clean, professional UI using Tailwind CSS
- Real-time preview of documents
- Payment section with:
  * Total amount input with automatic formatting
  * Deposit percentage selector (default 50%)
  * QR code generation for payments
- Document controls:
  * Preview/Update Preview buttons
  * Generate ODT/PDF buttons
  * Voice input button with recording indicator
  * Make Another button to start fresh
  * Shutdown button to close application
- Plumber selection dropdown
- Error and success message display system

Backend:
- /shutdown endpoint to close the application
- Document generation endpoints for ODT and PDF
- Payment processing endpoints
- File watching system for processing generated documents
- Voice-to-text processing
- Secure file handling with proper directory structure

Technical Requirements:
1. Error handling for all user interactions
2. Proper cleanup of temporary files
3. Maintain payment information across document regeneration
4. Support for both development and production environments
5. Comprehensive test suite using Jest
6. File upload handling
7. Proper shutdown sequence for the application

Directory Structure:
- /static: JavaScript, CSS, and other static assets
- /templates: HTML templates
- /uploads: Temporary file storage
- /tests: Test suite files
- Root level: Configuration files (package.json, babel.config.js, jest.config.js)

Security Considerations:
1. Secure handling of payment information
2. Protection against unauthorized shutdowns
3. Proper file permissions for uploaded content
4. Sanitization of user input

The application should be designed for local use, running on localhost with proper error handling and user feedback throughout all operations.
