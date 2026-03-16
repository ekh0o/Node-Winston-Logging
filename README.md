# Winston Logging Example (Task 1)

This project demonstrates how to implement logging in a Node.js application using the Winston logging library.

## Requirements

- Node.js 18
- Winston 3.11.0

## Installation

Clone the repository:

`git clone https://github.com/ekh0o/Node-Winston-Logging/`

Navigate to the project directory:

`cd node-winston-logging`

Install dependencies:

`npm install`

## Running the Application

Run the application with:

`node src/main.js`

## Logging Functionality

The application logs messages using the Winston logging library.

Log levels used:

- info
- warn
- error

Example log messages:

logger.log('info', 'This is an informational message.');
logger.warn('This is a warning message.');
logger.error('This is an error message.');

## Log Configuration

The logger is configured in:

`src/logger.js`

The logger uses:

- Console transport
- File transport

Log format:

- timestamp
- JSON

## Log Files

Log files are stored in the `logs` directory:

logs/error.log  
logs/combined.log

error.log contains only error level messages.

combined.log contains all log messages.

## Project Structure

.\
├── .gitignore\
├── package-lock.json\
├── package.json\
├── README.md\
└── src\
    ├── logger.js\
    └── main.js\

## .gitignore

The following files are ignored to prevent reproducible or environment-specific data from being stored in the repository:

node_modules/
logs/
.env
.DS_Store
