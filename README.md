<div align="center">
  <img src="https://res.cloudinary.com/db1tiugho/image/upload/f_auto,q_auto:eco,r_max/v1772947434/LOGO_oprvqu.png" alt="Voice Note Studio Logo" width="120" height="120">
  
  # 🎙️ Voice Note Studio
  
  **Transform Your Audio into WhatsApp-Ready Voice Notes**
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![Made with HTML/CSS/JS](https://img.shields.io/badge/Made%20with-Vanilla%20Web-blue.svg)](https://developer.mozilla.org/en-US/docs/Web)
  [![Powered By FFmpeg](https://img.shields.io/badge/Powered%20By-FFmpeg%20WASM-green.svg)](https://ffmpegwasm.netlify.app/)

  ### [Live Demo](#) · [Report Bug](#) · [Request Feature](#)
</div>

---

## 🌟 Overview

**Voice Note Studio** is a beautiful, client-side web application designed to seamlessly bridge the gap between AI voice generation and real-world messaging apps. 

Have you ever generated the perfect AI voice clip on Hugging Face (like Qwen3-TTS), but found that WhatsApp rejects the file or sends it as an awkward MP3 attachment instead of a native, playable Voice Note snippet?

This elegant tool solves that problem entirely in your browser. It leverages the power of **FFmpeg WebAssembly** to instantly transcode any standard audio file into the high-efficiency `.opus` format structured perfectly for WhatsApp. **No server uploads required. 100% private.**

---

## 📸 Interface Preview

<div align="center">
  <img src="https://placehold.co/800x450/ffffff/0f172a.png?text=Voice+Note+Studio+Interface&font=Outfit" alt="Voice Note Studio UI" width="800">
  <p><em>Features a hyper-aesthetic, interactive particle physics background.</em></p>
</div>

---

## ✨ Features

- **🚀 Client-Side Processing**: Files never leave your device. The rendering engine downloads once and executes entirely within your browser memory.
- **📱 True Voice Note Formatting**: Encodes audio strictly to `libopus`, tricking WhatsApp into rendering your file as a natively recorded voice snippet rather than a generic audio message.
- **✨ Immersive UI**: Enjoy a premium, ad-free experience with a stunning glassmorphic design and an interactive, physics-based particle background that responds to your cursor.
- **⚡ Next-Gen Performance**: Drag-and-drop your audio to transcode it in milliseconds using WebAssembly technology.

---

## 🛠️ How It Works

1. **Step 1: Generation**  
   Click the "Clone Your Voice" button to navigate to a recommended Hugging Face Space (e.g., Qwen3-TTS) where you can easily generate and download your AI-synthesized audio.
2. **Step 2: Conversion**  
   Upload or drag your downloaded audio file into the dedicated dropzone in Voice Note Studio.
3. **Step 3: Export**  
   Click **Convert to Opus**. The built-in FFmpeg core parses your audio, optimizes it alongside the Opus codec, and generates your ready-to-share file. Download it and forward it to any WhatsApp chat!

---

## 💻 Technical Setup

To test visually on your native system before deployment, you simply need a lightweight HTTP server (to prevent CORS execution issues caused by loading WebAssembly from a `file://` protocol).

### Prerequisites
- Python 3.x installed (for the local server)

### Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/voice-note-studio.git
   cd voice-note-studio
   ```

2. Start the local server:
   ```bash
   python3 server.py
   ```

3. Open your browser and navigate to:
   ```text
   http://localhost:8000
   ```

---

## 🏗️ Deployment 

The project is fully static and Cloudflare Pages / Vercel ready!

1. **Static Hosting**: Simply point your hosting provider to the repository root directory.
2. **Routing Config**: If using Cloudflare Pages, the included `_headers` file ensures the FFmpeg worker executes without hitting Cross-Origin Isolater limitations. 

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to check [issues page](#) if you want to contribute.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

<div align="center">
  <p>Built with ❤️ for perfectly cloned voices.</p>
</div>
