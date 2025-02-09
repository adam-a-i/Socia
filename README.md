# Socia

![Socia Logo](socia_logo.png)

## Overview

Socia is a mobile application designed to help users improve their social and professional communication skills through interactive practice scenarios. The app features various modules including job interview preparation, presentation skills training, relationship communication, and social interaction practice. Users can engage in realistic conversation simulations with AI-powered feedback, record their responses, and receive detailed analysis of their speaking performance including metrics like confidence, clarity, pace, and tone. The app includes features such as daily challenges, progress tracking, and a chat interface with "Nerva" - an AI communication coach. It also offers specialized scenarios like salary negotiations, self-introductions, and public speaking practice, making it a comprehensive tool for developing social and professional communication competencies. The app has a modern, user-friendly interface with a dashboard that tracks user progress and achievements, making skill development both engaging and measurable.

## Pitch Video
[Watch the Pitch Video](https://github.com/user-attachments/assets/5ac81414-f369-4c4f-9fb8-8a795b935531)

## Setup Instructions

### Prerequisites

Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [Python 3](https://www.python.org/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)

### Frontend Setup

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/socia.git
    cd socia
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

3. **Start the Expo development server:**
    ```sh
    npx expo start
    ```

### Backend Setup

1. **Navigate to the backend directory:**
    ```sh
    cd backend
    ```

2. **Install Python dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

3. **Add environment variables:**
    Create a `.env` file in the `backend` directory with the following content:
    ```env
    AZURE_OPENAI_KEY=your_openai_key
    AZURE_OPENAI_ENDPOINT=your_openai_endpoint
    AZURE_OPENAI_VERSION=2023-05-15
    AZURE_SPEECH_KEY=your_speech_key
    AZURE_SPEECH_REGION=your_speech_region
    IP_ADDRESS=your_ip_address
    ```

    Follow these steps to obtain the required values:

    - **AZURE_OPENAI_KEY and AZURE_OPENAI_ENDPOINT:**
        1. Sign in to the [Azure Portal](https://portal.azure.com/).
        2. Navigate to your resource group and select the OpenAI service.
        3. Go to the "Keys and Endpoint" section.
        4. Copy the key and endpoint values.

    - **AZURE_SPEECH_KEY and AZURE_SPEECH_REGION:**
        1. Sign in to the [Azure Portal](https://portal.azure.com/).
        2. Navigate to your resource group and select the Speech service.
        3. Go to the "Keys and Endpoint" section.
        4. Copy the key and region values.

    - **IP_ADDRESS:**
        - **Windows:**
            1. Open Command Prompt.
            2. Run the command `ipconfig`.
            3. Look for the "IPv4 Address" under your active network connection.
        - **macOS:**
            1. Open Terminal.
            2. Run the command `ifconfig`.
            3. Look for the "inet" address under the relevant network interface.
        - **Ubuntu/Linux:**
            1. Open Terminal.
            2. Run the command `ip a`.
            3. Look for the "inet" address under the relevant network interface.

4. **Run the Flask server:**
    ```sh
    python3 main.py
    ```

### Running the App

To access the app on Android, iOS, or Windows phones:
1. Download the Expo Go app from your device's app store.
2. Scan the QR code displayed in the terminal after running `npx expo start`.

### Additional Notes

- The app uses React Native, ensuring a native look and feel on any mobile device.
- Regularly update dependencies to ensure compatibility and access to the latest features.

### Getting Environment Variables

#### Azure Keys
1. Sign in to the [Azure Portal](https://portal.azure.com/).
2. Navigate to your resource group and select the relevant services (OpenAI and Speech).
3. Copy the keys and endpoints from the "Keys and Endpoint" section.

#### IP Address
- **Windows:** Open Command Prompt and run `ipconfig`. Look for the "IPv4 Address".
- **macOS/Linux:** Open Terminal and run `ifconfig` or `ip a`. Look for the "inet" address under the relevant network interface.

Enjoy using Socia to enhance your communication skills!
