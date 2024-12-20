# KnowNonsense VR

KnowNonsense VR provides an immersive virtual reality environment to fact-check debates in real-time. The application processes spoken dialogue, identifies claims, and provides true/false feedback with explanations, displayed interactively within the VR experience.

---

## Features
- **Real-Time Fact-Checking**: Displays true/false feedback with explanations for claims made during a debate.
- **Interactive Transcript**: A transcript of the debate, along with fact-checking annotations, is presented and saved for later interaction.
- **Seamless Integration**: Works with a backend powered by FastAPI and a machine learning pipeline for accurate claim verification.

---

## How It Works
1. **Dialogue Recording**: The VR headset records the debate as audio.
2. **Speech-to-Text**: Audio is sent to the FastAPI backend for transcription.
3. **Claim Detection**: A fine-tuned Hugging Face model determines if a statement contains an objective or statistical claim.
4. **Fact-Checking**: Claims are verified using Google's LLaMA, which provides sources and explanations.
5. **Visualization**: Results are displayed in VR in real-time and stored for later access.
