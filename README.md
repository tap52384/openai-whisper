# openai-whisper

Free application [from OpenAI](https://github.com/openai/whisper) for creating a transcript from an audio file with timestamps. Installs on your computer but downloads a model,
which can be useful for processing files locally without uploading sensitive
files to the Internet.

```bash
# Create a virtualenv
python3 -m venv .venv

# Activate the virtualenv
source .venv/bin/activate

# Upgrade pip
pip install --upgrade pip

# Install openai-whisper and its required packages
pip install -U openai-whisper

# Transcribe a file into all available formats
# "medium" is the best balance of quality and speed, but it is still slow,
# transcribing almost a second of audio per second
# If the model is not already on your computer, it is downloaded
whisper file.m4a --model medium --output_format all --language en
```
