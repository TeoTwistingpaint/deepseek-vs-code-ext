# DeepSeek AI VS Code Extension

This is a **VS Code extension** that allows you to chat with **DeepSeek AI** directly inside your editor.

## 🚀 Installation & Setup

### 1️⃣ Install Ollama
To run DeepSeek AI locally, you need to install **Ollama**:

➡️ **Download and install Ollama** from [the official website](https://ollama.com).

### 2️⃣ Select and Download a Model
DeepSeek AI offers multiple model sizes. Choose one from the **[DeepSeek model library](https://ollama.com/library/deepseek-r1)** and install it.

For example, to install the smallest model (**1.5B** parameters), run:
```sh
ollama run deepseek-r1:1.5b
```
This will download the model if it's not already installed.

### 3️⃣ Run the Extension in VS Code

#### 🔹 Start Debugging the Extension
1. Open the extension project in **VS Code**.
2. Press **Cmd + P** (or **Ctrl + P** on Windows/Linux) and type:
   ```
   >Debug: Select and Start Debugging
   ```
3. Choose the **Run Extension** option.
4. This will open a new VS Code window where the extension is running.

#### 🔹 Start a Chat with DeepSeek AI
1. In the **new VS Code window**, press **Cmd + P** (or **Ctrl + P**) and type:
   ```
   >Chat with DeepSeek
   ```
2. A chat window will open where you can interact with DeepSeek AI!

## 🛠️ Features
- **Chat with DeepSeek AI** directly in VS Code
- **Streamed responses** for a smoother experience
- **Supports multiple DeepSeek model sizes** (1.5B, 7B, etc.)

## 📌 Notes
- Make sure **Ollama** is running in the background.
- If you encounter issues, try restarting VS Code or running `ollama run deepseek-r1:1.5b` again to ensure the model is loaded.

Happy coding! 🚀

