# DeepSeek AI Chat - VS Code Extension

This VS Code extension allows you to chat with **DeepSeek AI** directly from your editor. It leverages [Ollama](https://ollama.com) to run the AI model locally on your device.

## 🚀 Setup Instructions

### 1️⃣ Install Ollama
First, install Ollama on your system by downloading it from [ollama.com](https://ollama.com).

### 2️⃣ Pull the DeepSeek Model
Choose a model version from the [DeepSeek Model Library](https://ollama.com/library/deepseek-r1) and pull it using the command:

For example, to install the **smallest (1.5B) model**, run:
```sh
ollama pull deepseek-r1:1.5b
```
Or, for the **larger (7B) model**:
```sh
ollama pull deepseek-r1:7b
```

### 3️⃣ Run the VS Code Extension
1. Open VS Code.
2. Press **Cmd + P** (**Ctrl + P** on Windows/Linux) and search for:
   ```
   >Debug: Select and Start Debugging
   ```
3. In the new VS Code window, press **Cmd + P** (**Ctrl + P**) and search for:
   ```
   >Chat with DeepSeek
   ```
4. Start chatting with DeepSeek AI! 🎉

## ⚠️ Important: Update the Code with Your Installed Model

In the extension code, **make sure to specify the model you installed**. Modify this part accordingly:

```typescript
const streamResponse = await ollama.chat({
  model: "deepseek-r1:1.5b", // update here with the DeepSeek model you've installed
  messages: [{ role: "user", content: userPrompt }],
  stream: true,
});
```

If you've installed a different model version (e.g., `7b`), change the line to:
```typescript
model: "deepseek-r1:7b"
```

## ✅ Verify Model Installation
If you encounter an error like:
```
Error: ResponseError: model "deepseek-r1:latest" not found, try pulling it first
```
Make sure to run:
```sh
ollama list
```
This should show the installed models. If the model isn't listed, **go back to Step 2 and pull it again**.

## 🛠️ Features
- **Chat with DeepSeek AI** directly in VS Code
- **Streamed responses** for a smoother experience
- **Supports multiple DeepSeek model sizes** (1.5B, 7B, etc.)

---
Enjoy chatting with DeepSeek AI inside VS Code! 🚀