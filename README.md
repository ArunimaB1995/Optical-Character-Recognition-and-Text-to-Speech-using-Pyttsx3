# Optical-Character-Recognition
OCR using Pytesseract
# Text-To-Speech
Using 'pyttsx3' and 'gtts'
```
pip install pyttsx3
```
or
```
conda install -c auto pyttsx
```
You can also use the Google-Text-To-Speech(GTTS) python package:
```
pip install gTTS
```
or
```
conda install -c tdido gtts-token
```
## Run file
```
Text-To-Speech/Text-To-Speech_demo

```
## Install required packages
Open new IPYNB file inside the Text-To-Speech folder; type the following code:

```
pip install -r requirements.txt
```

## Image folder
```
Text-To-Speech/images/
```

You can add more files of .PNG, .TIFF, .JPG extension, for the tesseract to work on

## Tesseract.exe
Download 'tesseract-ocr-setup-3.02.02' and perform installation or you can download the setup file from: 
https://osdn.net/projects/sfnet_tesseract-ocr-alt/downloads/tesseract-ocr-setup-3.02.02.exe/

Add the file location after setup and installation in the Text-To-Speech-demo.ipynb file as:
```
pytesseract.pytesseract.tesseract_cmd = 'path/to/tesseract.exe'
```
The pyttsx3 module supports two voices first is female and the second is male which is provided by “sapi5” for windows. It supports three TTS engines : sapi5 – SAPI5 on Windows. You can view the in-built voice and their ids using these lines of code and change accordingly to your preferances:
https://www.geeksforgeeks.org/text-to-speech-changing-voice-in-python/
or follow this blog:
https://puneet166.medium.com/how-to-added-more-speakers-and-voices-in-pyttsx3-offline-text-to-speech-812c83d14c13
for adding voices in the pyttsx3 default voice_list
```
for voice in voices:
    engine.setProperty('voice', voices[0].id) #'voices[1].id' will play female voice
```
'Voices[2].id' will play the voice added into:
    Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Speech\Voices\Tokens\   
    after following the instructions in the medium-blog mentioned above.

