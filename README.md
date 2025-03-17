# GPTCaller_free
This is the free version of GPTCaller.

This application provides a client interface for interacting with locally hosted Large Language Models (LLMs) via API calls.  It also supports integration with OpenAI's ChatGPT if you have an API key.

![app_screen_shot.png]

## Overview
This client allows you to easily connect to and query various LLMs, including those run locally using tools like [Ollama](https://ollama.com/).  It provides a streamlined interface for managing connections, viewing chat history, and querying models with simple text or documents.

### Key Features
*   **LLM Connection Management:** Easily add, edit, and manage connections to different LLM APIs.
*   **Chat History:**  View and manage your conversation history with each LLM.  Export history to `.md` files for archiving or further analysis.
*   **Document Querying:**  Provide a simple document as context for your queries, allowing the LLM to answer questions based on the document's content.
*   **Ollama Support:** Seamlessly integrate with Ollama to download and run various LLM models locally.

## Getting Started

### Prerequisites

*   macOS
*   An LLM server (e.g., Ollama, a self-hosted model, or access to OpenAI's API)
## Installation
1. **Download the DMG:**
   Download the latest DMG file from the [Releases page](https://github.com/[your username]/[your repository]/releases).

2. **Mount the DMG:**
   Double-click the downloaded DMG file to mount it.

3. **Drag and Drop:**
   Drag the application icon from the mounted DMG to your Applications folder.

4. **Launch the Application:**
   Open the application from your Applications folder. You may be prompted to confirm that you want to open an application downloaded from the internet.

**Important Note:**
*   If you encounter any issues during installation, please check the [Troubleshooting](TROUBLESHOOTING.md) section or create an issue on the [GitHub repository](https://github.com/[your username]/[your repository]/issues).

## Configuration

To configure the application, follow these steps:

1. **Launch the Application:** Start the application.
2. **Click the Gear Icon:**  Click the settings (gear) icon located in the top-right corner of the application window.
3. **Enter the Following Information:**
   * **Server Name:** Enter a descriptive name for your LLM server. This name helps you identify the server within the application.  You can choose any name you like.
   * **API Key:** Enter your API key.  Note that some servers, such as Ollama, do not require an API key.
   * **Server Model:** Enter the name of the LLM model you want to use (e.g., `gemma-7b`, `llama-3-8b`, `gpt-4o`).
   * **End Point:** Enter the connection URL for the server (e.g., `http://localhost:11434` for Ollama, `https://api.openai.com/v1/chat/completion` for OpenAI's Chat-GPT).
   * **Temperature:** Enter your desired temperature value. This controls the randomness of the generated text.  Lower values (e.g., 0.1) produce more predictable text, while higher values (e.g., 0.8) produce more creative text.

**Note:** After changing these settings, click **Save** to apply the changes. A restart is not required; the settings will be applied immediately.

![[new_server.png]]
![[server_setting.png]]
![[server_list.png]]
### Using ChatGPT
If you have an OpenAI API key, you can add a connection of type "OpenAI" and enter your API key.  The application will then use the OpenAI API for your queries.

## Features in Detail

#### Chat History
The application stores your chat history for each LLM connection. You can view, delete, and export your chat history to `.md` files for archiving or further analysis.

#### Document Querying
You can provide a simple document (e.g., a `.txt` or `.pdf` file) as context for your queries. The application will send the document along with your query to the LLM, allowing it to answer questions based on the document's content.

## Acknowledgements
*   [Ollama](https://ollama.com/) - For providing a simple way to run LLMs locally.
*   [OpenAI](https://openai.com/) - For providing access to powerful language models.

