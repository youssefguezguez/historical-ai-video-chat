# Historical AI Video Chat

A prototype web app for talking with an AI-simulated historical figure, Hannibal Barca, in a
"video call" in the browser. Built during an AI internship at Golden Madina (Nabeul, Tunisia)
in summer 2024.

**How it works**
- **Conversation:** OpenAI chat API with a role-play system prompt. Hannibal answers briefly,
  in English, French or Arabic.
- **Voice:** questions can be spoken (browser speech recognition), and answers are read aloud
  with ElevenLabs multilingual text-to-speech.
- **Avatar:** an animated 3D model of Hannibal rendered with three.js (GLTF/Draco).
- **Call view:** the user's webcam via WebRTC, plus the conversation history.

**Stack:** Python, Flask, Flask-SocketIO, OpenAI API, ElevenLabs API, JavaScript, three.js, WebRTC.

**Status:** prototype, not deployed. Only Hannibal is implemented; the other characters on the
home page are placeholders. The 3D model file (~96 MB) is not included in the repository.

## Run locally

```bash
pip install -r requirements.txt
# put your keys in config.py: OPENAI_API_KEY, ELEVENLABS_API_KEY
# add a GLTF model at static/models/untitled.glb
python app.py
```
