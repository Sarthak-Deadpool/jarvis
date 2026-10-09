<!-- @format -->

# JARVIS — Voice Assistant

A Python-based voice assistant project that aims to recognize voice commands through a microphone and perform tasks based on user instructions.

## Project Status

**Current milestone:** Initial environment setup

- [x] Python virtual environment created
- [x] SpeechRecognition installed
- [x] PyAudio installed
- [ ] Microphone input tested
- [ ] Speech recognition tested
- [ ] Voice command processing implemented
- [ ] Assistant features implemented

## Tech Stack

- **Language:** Python 3.13
- **Speech Recognition:** SpeechRecognition
- **Microphone Input:** PyAudio
- **Environment Management:** Python `venv`
- **Terminal:** Windows PowerShell

## Prerequisites

- Windows 10 or Windows 11
- Python 3.13
- Working microphone
- Internet connection for Google speech recognition

## Project Setup

### 1. Clone or open the project

Open PowerShell and navigate to the project directory:

```powershell
cd C:\Users\Sarthak\Desktop\jarvis
```

### 2. Create a virtual environment

```powershell
py -3.13 -m venv .venv
```

### 3. Activate the virtual environment

```powershell
.\.venv\Scripts\Activate.ps1
```

### 4. Upgrade pip

```powershell
python -m pip install --upgrade pip
```

### 5. Install dependencies

```powershell
python -m pip install SpeechRecognition PyAudio
```

## Installed Libraries

| Library           | Purpose                                            |
| ----------------- | -------------------------------------------------- |
| SpeechRecognition | Captures and processes speech recognition requests |
| PyAudio           | Provides microphone audio input                    |
| typing-extensions | Provides typing compatibility features             |
| standard-aifc     | Supports AIFF audio file handling                  |
| audioop-lts       | Provides audio processing compatibility            |
| standard-chunk    | Supports chunk-based audio file handling           |

## Verify Installation

Run the following command:

```powershell
python -c "import speech_recognition as sr; import pyaudio; print('Audio libraries working!')"
```

If the command prints `Audio libraries working!`, both primary libraries can be imported successfully.

## Running the Project

The microphone test script and main assistant application are not implemented yet.

Once these files are created, run the appropriate script from the activated virtual environment:

```powershell
python test_mic.py
```

## Troubleshooting

### PyAudio installation fails

Make sure the virtual environment uses Python 3.13:

```powershell
python --version
```

Then install the dependencies again:

```powershell
python -m pip install SpeechRecognition PyAudio
```

### Microphone not detected

- Check Windows microphone permissions.
- Verify that the correct input device is selected.
- Ensure the microphone is connected and working.

### Speech recognition service error

Check your internet connection. Google speech recognition requests require internet access.

## Future Improvements

- [ ] Test live microphone input
- [ ] Convert speech into text
- [ ] Process voice commands
- [ ] Add text-to-speech responses
- [ ] Integrate useful desktop commands
- [ ] Add error handling and logging
- [ ] Organize the project into reusable modules

## License

No license has been selected yet. Add a license before distributing the project publicly.
