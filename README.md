# Historical AI Video Chat

A prototype web app for video chats with AI-simulated historical figures, built solo during
my AI internship at Golden Madina (Nabeul, Tunisia), May–August 2024.

- **Role-play:** a GPT model fine-tuned through the OpenAI API plays each figure (Hannibal
  Barca, Mago I of Carthage, Elissa) and answers briefly in English, French or Arabic.
- **3D avatars:** each figure is rendered as an animated 3D avatar in the browser with three.js.
- **Video call:** WebRTC call view, with spoken questions (speech recognition) and spoken
  answers (ElevenLabs multilingual text-to-speech).

**Stack:** Python, Flask, LangChain, WebRTC, OpenAI API, ElevenLabs, three.js

**Status:** prototype, not deployed. This repository holds the prompt-based version of the
role-play (gpt-3.5-turbo) with Hannibal implemented; the 3D model file (~96 MB) is not included.

## Run locally

```bash
pip install -r requirements.txt
# put your keys in config.py: OPENAI_API_KEY, ELEVENLABS_API_KEY
# add a GLTF model at static/models/untitled.glb
python app.py
```
