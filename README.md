# Optical-Character-Recognition
OCR using Pytesseract
# Text-To-Speech
Using 'pyttsx3' and 'gtts'

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
Download 'tesseract-ocr-setup-3.02.02' inside the Text-To-Speech folder and perform installation or you can download the setup file from: 
https://osdn.net/projects/sfnet_tesseract-ocr-alt/downloads/tesseract-ocr-setup-3.02.02.exe/
Add the installed file location in the Text-To-Speech-demo.ipynb file as:
```
pytesseract.pytesseract.tesseract_cmd = 'path/to/tesseract.exe'
```

