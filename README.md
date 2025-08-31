# robloxbot
 An intelligent voice-controlled assistant for Roblox that listens to your commands, responds in chat, and can even detect and interact with players on screen.  


## ✨ Features  
- 🎙 **Voice commands** with trigger words: `"Alice"`, `"Alexa"`, `"Here"`  
- 🤖 **AI-powered responses** via Groq API (LLaMA model)  
- ⌨️ **Auto chat typing** – the bot writes in Roblox chat like a real player  
- 👀 **Object & player detection** using YOLO + custom ML model (`best.pt`)  
- 🕹 **Automated interactions**: moves mouse, clicks players, scrolls camera if needed  
- 🌐 **Hybrid speech recognition**: Whisper + online transcription (Clipto.com)  

---

## 🛠 Tech Stack  
- **Python**  
- **OpenAI Whisper** – offline speech recognition  
- **Selenium** – automated browser for transcription  
- **YOLO (Ultralytics) + PyTorch** – object detection  
- **Groq API (LLaMA)** – natural language responses  
- **PyAutoGUI & Pynput** – keyboard/mouse automation  
- **PIL.ImageGrab** – screen capturing  

---

## 📂 Project Structure  

roblox bot/
│── main.py # Main loop: listens, processes, executes
│── detect_speech.py # Trigger word detection + voice recording
│── speech_to_text.py # Converts voice commands to text (via Clipto)
│── ask_groq.py # Sends command to Groq API & types response
│── detect_go.py # YOLO-based player/object detection
│── best.pt # Custom trained YOLO model
│── command.wav # Example voice command
│── screenshot.png # Project screenshot

## 🚀 How It Works  
1. 🎧 Bot listens for trigger words: `"Alice"`, `"Alexa"`, `"Here"`.  
2. If `"Alice"`/`"Alexa"` → records your voice command.  
3. 🎙 Command is transcribed into text (Whisper + Clipto).  
4. 🤖 Text is sent to **Groq API (LLaMA)** → short, funny, safe response.  
5. ⌨️ Bot types the response into Roblox chat automatically.  
6. If `"Here"` → YOLO model scans screen for players and clicks on them and it moves in thst direction.  

---

## 📸 Preview  
![screenshot](roblox%20bot/screenshot.png)  

---

## ⚠️ Disclaimer  
This project is for **educational purposes only**.  
Using automation or bots in Roblox may violate their Terms of Service.  
Use responsibly!  

---

💡 Contributions, ideas, and improvements are welcome!  

