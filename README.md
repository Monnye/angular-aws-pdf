# PDF Management Application

This project is an Angular-based application for managing PDF files, providing features such as viewing, downloading, uploading, and requesting missing PDFs. It integrates with AWS for secure and scalable file storage.

## Table of Contents

1. [Development server](#development-server)
2. [Code scaffolding](#code-scaffolding)
3. [Build](#build)
4. [Running unit tests](#running-unit-tests)
5. [Running end-to-end tests](#running-end-to-end-tests)
6. [Usage](#usage)
7. [API Endpoints](#api-endpoints)
8. [AWS Integration](#aws-integration)
9. [State Management](#state-management)
10. [Authentication](#authentication)
11. [Contributing](#contributing)
12. [License](#license)

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Usage

- **Authentication:**
  - Log in to access the PDF Management Dashboard.
- **PDF Management:**
  - View, download, upload, and request missing PDFs from the Dashboard.

## API Endpoints

- **Authentication API:**
  - `POST /api/auth/login`: Authenticate user and generate JWT token.
- **PDF Management APIs:**
  - `GET /api/pdf/all`: Retrieve list of available PDFs.
  - `GET /api/pdf/:id/view`: Retrieve a specific PDF for viewing.
  - `GET /api/pdf/:id/download`: Retrieve a specific PDF for downloading.
  - `POST /api/pdf/upload`: Upload a new PDF file.
- **Request Missing PDF API:**
  - `POST /api/request/pdf`: Record a user's request for a missing PDF.
- **AWS S3 Integration API:**
  - `POST /api/aws/upload`: Upload a file to AWS S3.
  - `GET /api/aws/:filename/download`: Retrieve a file from AWS S3 for downloading.

## AWS Integration

- Set up an AWS account.
- Configure S3 bucket for PDF storage.
- Integrate AWS SDK for JavaScript in the browser.

## State Management

- Use NGXS for state management.
- Define states, actions, and selectors.

## Authentication

- Implement JWT token-based authentication.
- Secure API endpoints for authentication.

## Contributing

We welcome contributions! Feel free to submit issues or pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
