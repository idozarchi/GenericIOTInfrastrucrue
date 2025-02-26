# Generic IoT Infrastructure

This project is a versatile IoT infrastructure aimed at helping users manage data from their IoT devices. The entire project was developed from scratch with minimal reliance on external libraries.

## Main Components

1. **Website**
    - Developed using Next.js and Tomcat.
    - Offers a user-friendly interface for IoT data management.

2. **Gateway Server**
    - Features the `ConnectionService` supporting HTTP, TCP, and UDP protocols.
    - Includes the `RequestProcessingService` which uses a thread pool for efficient request handling.

## Directory Structure

- `/website`
  - Contains the Next.js and Tomcat files for the web interface.
  
- `/gateway-server`
  - `ConnectionService`
     - Manages connections using HTTP, TCP, and UDP protocols.
  - `RequestProcessingService`
     - Processes incoming requests with a thread pool.

- `/config`
  - Contains configuration files for the project, including settings for the Gateway Server and the website.

- `/scripts`
  - Includes scripts for setting up, deploying, and managing the project.

- `/docs`
  - Documentation files providing detailed information about the project, its components, and how to use and contribute to it.

## Getting Started

1. **Clone the repository**
    ```bash
    git clone <repository-url>
    ```

2. **Navigate to the project directory**
    ```bash
    cd Generic-IoT-Infrastructure
    ```

3. **Install dependencies for the website**
    ```bash
    cd website
    npm install
    ```

4. **Run the website**
    ```bash
    npm run dev
    ```

5. **Start the Gateway Server**
    ```bash
    cd ../gateway-server
    # Command to start the server (e.g., java -jar gateway-server.jar)
    ```

## Usage

- Access the website at `http://localhost:3000` to manage your IoT data.
- The Gateway Server will handle incoming connections and process requests using the specified protocols.

## Project Overview

The Generic IoT Infrastructure project provides a comprehensive platform for managing data from IoT devices. It is designed to be scalable and efficient, supporting multiple networking protocols and ensuring smooth data processing. The entire project was developed from scratch with minimal reliance on external libraries.

### Internal Components

1. **Website**
    - Built with Next.js for the frontend and Tomcat for the backend, the website offers an intuitive interface for users to manage their IoT data. It allows users to view, analyze, and control their IoT devices and the data they generate.

2. **Gateway Server**
    - The Gateway Server serves as the bridge between IoT devices and the data management system. It includes:
        - **ConnectionService**: Handles connections from IoT devices using HTTP, TCP, and UDP protocols, ensuring compatibility with various devices.
        - **RequestProcessingService**: Manages the processing of incoming requests using a thread pool, allowing for concurrent handling of multiple requests and enhancing system efficiency.
