# HotSeat - AI Interviewer

# HotSeat 🔥

A voice-first AI mock interview tool for CS students. Practice technical interviews by actually talking through problems out loud — not typing solutions in silence.

---

## The problem

You can grind 200 LeetCode problems and still freeze in a real interview. The gap isn't knowing the algorithm — it's performing under conversational pressure. Talking through your thinking while someone interrupts, asks why, and pushes back when you hand-wave is a completely different skill. HotSeat trains that skill.

---

## What it does

- Asks you a technical interview question out loud
- Listens to your answer via voice (push-to-talk)
- Pushes back when you're vague or incorrect
- Gives graduated hints only when you're genuinely stuck — never the full answer
- Asks follow-up questions if you finish early
- Ends the session and tells you what to work on

---

## Tech stack

| Layer | Tool |
|---|---|
| Frontend | React + Vite + Tailwind |
| Backend | FastAPI (Python) |
| Voice transport | LiveKit (WebRTC) |
| Speech to text | Groq Whisper |
| LLM | Groq — Llama 3.3 70b |
| Text to speech | Browser Web Speech API |
| Deployment | Railway |

---

## Status

Currently in active development. V1.0 is the core voice loop — push-to-talk, one question per session, basic end screen. No account required.

**V1.0 (in progress)**
- [x] Project planning and architecture
- [ ] Question bank (hardcoded JSON)
- [ ] FastAPI backend + LiveKit integration
- [ ] React frontend
- [ ] Deployed on Railway

**V1.1 (next)**
- [ ] Postgres session persistence
- [ ] Post-session diagnostic report
- [ ] Open mic + interruption handling (Deepgram streaming)
- [ ] User accounts and history

---

## Running locally

> Setup instructions coming once V1.0 is built.

---

## Why voice?

Typing removes the pressure. In a real interview you have to think out loud, handle interruptions, and communicate your reasoning in real time. Every existing mock interview tool lets you type. HotSeat doesn't.
