# Whisper-based audio to text transcriber with speaker identification

## Setup
`FFMPEG` and `Cython` are needed as prerquisites to install the requirements
```
pip install cython
```
or
```
sudo apt update && sudo apt install cython3
```
```
# on Ubuntu or Debian
sudo apt update && sudo apt install ffmpeg

# on MacOS using Homebrew (https://brew.sh/)
brew install ffmpeg

# on Windows using Chocolatey (https://chocolatey.org/)
choco install ffmpeg

# on Windows using Scoop (https://scoop.sh/)
scoop install ffmpeg
```
```
pip install -r requirements.txt
```
## Usage 

Put the audio file you want to transcribe in the same folder and run
```
python diarize.py -a "audio.mp3"
```

## Command Line Options

- `-a AUDIO_FILE_NAME`: The name of the audio file to be processed
- `--no-stem`: Disables source separation
- `--whisper-model`: The model to be used for ASR, default is `medium.en`
- `--suppress_numerals`: Transcribes numbers in their pronounced letters instead of digits, improves alignment accuracy
