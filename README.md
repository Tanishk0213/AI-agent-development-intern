# AI Voice Sales Bot for TaskFlow CRM

## Project Overview
The **AI Voice Sales Bot** is an AI-powered sales assistant designed to interact with potential customers, answer product-related questions, identify demo requests, and generate call summaries.

The application provides a web-based interface built using Gradio and supports text-based conversations, with voice-related features for speech transcription and audio generation.

## Features
- AI-powered sales conversations
- Customer recording-consent prompt
- Text-based message input
- Voice input interface
- Speech-to-text transcription using Faster-Whisper
- AI responses using the Groq API
- Audio response generation using Edge TTS
- Automatic call summary
- Customer requirements and objections tracking
- Sales status detection, such as demo requested
- Call duration and call history
- Transcript storage during the current runtime

## Technologies Used
- **Python** – Core programming language
- **Google Colab** – Development and execution environment
- **Gradio** – Web-based user interface
- **Groq API** – AI-powered conversation responses
- **Faster-Whisper** – Speech-to-text transcription
- **Edge TTS** – Text-to-speech audio generation
- **Pydub** – Audio processing

## Project Workflow
1. Start the call from the web interface.
2. Ask for customer consent before saving audio.
3. Receive customer messages through text or voice input.
4. Process the message and generate a sales response.
5. Identify customer requirements, objections, and demo interest.
6. End the call and generate a summary.
7. Review the sales status, next steps, and call history.

## Installation and Setup

### 1. Open the Notebook
Upload the project notebook to Google Colab and run the cells in order.

### 2. Configure the API Key
Create a Groq API key from:

https://console.groq.com/keys

Enter the key when prompted by the notebook. Keep the key private.

### 3. Install Dependencies
The notebook installs the required Python packages automatically.

### 4. Launch the Application
Run the Gradio launch cell and open the generated web link.

### 5. Test the Application
Try these sample messages:
- `I want to know about your CRM product.`
- `What is the pricing?`
- `Can I book a demo?`
- `I need to discuss with my manager.`

End the call and review the generated summary.

## Sample Use Case
A potential customer wants to learn about TaskFlow CRM. The bot explains the product's trial offer, responds to questions, recognizes the customer's interest in a demo, and marks the sales status as **Demo Requested**.

## Privacy and Security
- Obtain appropriate consent before recording customer audio.
- Do not use real customer information without authorization.
- Never publish API keys in source code or public repositories.
- Call history and recordings may be temporary and can disappear when the Colab runtime resets.
- Follow applicable privacy and data-protection requirements.

## Current Limitations
- Microphone availability depends on browser permissions and device configuration.
- Audio recording may not be saved if consent is not granted or audio generation is unavailable.
- Demo requests are identified by the bot; an actual calendar booking or confirmation requires an additional booking integration.
- Persistent storage requires a database or another storage solution.

## Future Enhancements
- Integrate calendar-based demo booking.
- Add CRM database integration.
- Implement persistent call-history storage.
- Improve microphone and audio-recording reliability.
- Add customer lead scoring and follow-up reminders.
- Support multiple languages.

## Conclusion
The AI Voice Sales Bot demonstrates how AI, speech technologies, and a web interface can automate initial sales conversations, identify potential leads, and assist sales teams with follow-up activities.
