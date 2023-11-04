# Whisper-based audio to text transcriber with speaker identification

## Setup
`FFMPEG` and `Cython` are needed as prerquisites to install the requirements. You will also need an computer with NVIDA GPU that supports CUDA.
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

Put the audio file you want to transcribe in the audio folder and run. The scripts should be saved in the transcripts folder
```
python transcribe.py
```
