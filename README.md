# AI Head Project

An AI that lives inside a robot head: a Wheatley-style personality that talks, looks around and reacts.

## How it works

- **PC (RTX 4080):** runs the heavy parts. Speech-to-text (Whisper), the LLM (local via Ollama), and text-to-speech (Piper).
- **Raspberry Pi:** the small brain. It handles the mic, the speaker and Wi-Fi to the PC, and sends movement commands to the eye board.
- **Eye mechanism:** Will Cogley's EyeMech ε3.2 with 6x MG90S servos, driven by the RP2040 EyeMech board over USB through a powered hub.

## Folders

- `sim/`: browser simulator for previewing the head's expressions and servo poses. Open `sim/index.html` in any browser.
- `pc-server/`: AI server for the PC (coming soon)
- `pi-client/`: Raspberry Pi client (coming soon)
- `eye-board/`: command-mode firmware for the EyeMech board (coming soon)

## Credits

The eye mechanism and controller board are by [Will Cogley](https://www.willcogley.com), licensed CC BY-NC-SA 4.0. His design files are not included in this repo.
