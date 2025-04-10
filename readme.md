
# Virtual Companion

An AI-Powered Virtual Assistant for Real-Time Live Interaction


## Overview
The Virtual Companion is an autonomous, AI-driven virtual assistant designed for real-time engagement in live streaming, education, and customer support. It combines DeepSeek-V2 (for natural conversations), Microsoft Azure TTS (for lifelike speech), and VTube Studio (for expressive facial animations) to create a dynamic digital persona that interacts naturally with audiences no human operators required.
## Key Features
✅ Real-Time AI Chat – Powered by DeepSeek-V2 for low-latency, context-aware responses.

✅ Natural Voice & Lip-Sync – Azure TTS + VTube Studio for fluid speech and animations.

✅ Streamer-Friendly – Seamless OBS Studio integration with customizable UI controls.

✅ Cost-Efficient – Hybrid local (Ollama/DeepSeek) + cloud (Azure) architecture.
## Use Cases
🎥 Live Streaming – AI co-hosts for interactive broadcasts.

📚 Education – Virtual tutors for remote learning.

🛎️ Customer Support – 24/7 AI assistants with branded avatars.
## Tech Stack

**AI Backend:** DeepSeek-V2 (via Ollama), Azure TTS

**Animation:** VTube Studio (2D avatar)

**Streaming:** OBS Studio + WebSockets (FastAPI)

**Cloud:** Microsoft Azure (Hosting, TTS)


## Prerequisites

- Windows operating system

- Administrator privileges for software installation

- Stable internet connection


## Installation

1. Install Required Software
Install Ollama
Download and install Ollama from the official website: https://ollama.ai

Install Visual Studio Code (VSCode)
Download and install from: https://code.visualstudio.com

Install FFmpeg

Download FFmpeg for Windows

Add FFmpeg to your system PATH environment variable

Install Steam

Download and install Steam from: https://store.steampowered.com

Create a Steam account if you don't have one

Install VTube Studio

Search for "VTube Studio" in Steam and install it

2. Setup Project Files
Download the project files from GitHub

Open the project in VSCode

Create a virtual environment:

```bash
python -m venv venv
```
    
Activate the virtual environment:

    Windows: .\venv\Scripts\activate

Install requirements:

    pip install -r requirements.txt

3. Configure Ollama
Close Ollama if it's already running

Run Llama3 model:

    ollama run llama3

In a separate PowerShell terminal, start Ollama server:

    ollama serve

4. Run the Application
Open a new PowerShell terminal

Run the main application:

    python main.py

5. Setup VTube Studio with Audio
Install VTS Desktop Audio Plugin
Download from: https://lualucky.itch.io/vts-desktop-audio-plugin

Launch VTube Studio

Select any free avatar from the available options

Open VTS Desktop Audio

Connect it to VTube Studio through the settings menu

Configure mouth movement

Connect the avatar's mouth movement to Desktop Audio input

Troubleshooting
If Ollama fails to run, ensure it's properly installed and has internet access

For audio issues, check your system's audio input settings

Make sure all paths are correctly set in environment variables

Support
For additional help, please refer to:

VTube Studio documentation

Ollama GitHub repository

Project GitHub issues page