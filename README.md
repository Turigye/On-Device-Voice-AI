# On-Device-Voice-AI
This project performs on-device text-to-speech by listening to a microphone recording from the user and transcribing it into text that is then fed to ChatGPT which in turn, responds to the user with a voice output allowing for a free-flowing conversation on the device.

Creating Your Own Voice-Powered Assistant Using NodeJS

In this guide, I'll demonstrate how to craft a conversational bot that responds to your voice within a mere five minutes, leveraging NodeJS. This project is an excellent introduction to OpenAI's Whisper API for voice recognition and the TTS (Text-to-Speech) technology for audible responses.

**Prerequisites for the Project:**

- Ensure Node.js is set up on your system.
- Acquire an OpenAI API key by registering on the OpenAI platform.
- Have a fundamental grasp of JavaScript and Node.js.

**Necessary Node.js Packages:**

Before we begin, you will need to install several NPM packages:

- `node-microphone`
- `fs`
- `fluent-ffmpeg`
- `ffmpeg-static`
- `readline`
- `axios`
- `form-data`
- `speaker`
- `openai`
- `dotenv`

To install these packages, use the command `yarn add openai` or the equivalent npm command, depending on your preference.

**How the Voice-Activated Assistant Functions:**

The assistant's operation is straightforward but efficient:

1. It captures your voice input.
2. Transcribes the audio to text using the Whisper API.
3. Sends the text to OpenAI's chat completions endpoint for processing.
4. Converts the assistant's textual response into speech through TTS.
5. Plays the spoken response.

This process emulates a natural dialogue with a digital companion.

**Code Implementation Steps:**

1. Begin by creating a `.env` file to securely store your OpenAI API key, like so:

```plaintext
# .env file
OPENAI_API_KEY="YOUR OPENAI API KEY HERE"
```

2. Download the `chat.js` file and place it in your project directory alongside the `.env` file.

3. Customize the TTS voice or the chatbot's system prompt to vary the interaction experience.

**Environment Setup:**

Install the required Node.js modules and address any system-specific setup needs, such as configuring ffmpeg if it isn't already. Ensure your terminal has permission to output sound.

**Launching Your Assistant:**

To test your voice-activated assistant:

1. Open your terminal.
2. Navigate to the directory containing your project files.
3. Execute the command `node chat.js`.

You will then be able to engage with your assistant, asking questions and receiving responses in a conversational format, all through voice commands and replies.
