<p align="center">
  <img src="Logo/video-streaming.png" alt="Logo" width="150" />
</p>

# Video Streaming Web App

This app lets you upload, store, and stream your videos seamlessly. It's built with a modern tech stack and designed for easy setup and use.

**Here's what it does:**

* **Upload and Manage:** Easily upload your video files and their details (title, description, etc.).
* **HLS Streaming:**  Converts your videos into HLS format using FFmpeg for smooth playback on any device.
* **Efficient Retrieval:** Quickly access and retrieve your stored video metadata.
* **Robust Error Handling:**  Ensures a reliable experience by gracefully handling any video processing errors.

## Tech Stack

* **Frontend:** React JS, Tailwind CSS (for a sleek and responsive user interface)
* **Backend:** Spring Boot (for a robust and scalable backend), MySQL/PostgreSQL (for reliable data storage)

## Run Locally

1. Clone the project

```bash
  git clone https://github.com/makarandhinge/Video-Streaming-Web.git
```
2. Go to the backend project directory

```bash
  cd spring-stream-backend
```

3. Ensure that Java is installed on your system. You can verify this by running the following command

```bash
  java -version
```
4. Configure the Backend:
  - Update application.properties or application.yml in the backend directory
   ```bash
  # Database Configuration
spring.datasource.url=jdbc:mysql://localhost:3306/<database_name>
spring.datasource.username=<db_username>
spring.datasource.password=<db_password>

# Directory Configuration
files.video=<local_directory_for_videos>
file.video.hsl=<local_directory_for_hsl>
```
5. To build and run the Spring Boot application, you need Maven. If Maven is not installed, you can follow the installation instructions from [here](https://github.com/makarandhinge/Installtion-Guideline/blob/main/Maven.md)

- Build the project

```bash
  ./mvnw clean install
```
- Run the Spring Boot application

```bash
  ./mvnw spring-boot:run
```
The backend should now be running on http://localhost:8080.
6. Navigate to the Frontend Directory

```bash
  cd stream-front-end
```
6. Install Frontend Dependencies

Make sure you have Node.js installed. You can verify it with

```bash
node -v
npm -v
```
If Node.js is not installed, you can download it from [here](https://github.com/makarandhinge/Installtion-Guideline/blob/main/Node.md)

Run the following command to install the necessary dependencies for the frontend

```bash
 npm install
```

7. Start the React Development Server

To start the React development server (using Vite), use the following command:

```bash
npm run dev
```
The frontend should now be running on http://localhost:5173.
