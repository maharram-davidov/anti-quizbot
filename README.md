# QuizBot

A Python-based application that uses OCR (Optical Character Recognition) and AI to help answer quiz questions. The bot captures screenshots of quiz questions, processes them using EasyOCR, and gets answers using the Gemini AI API.

## Features

- Screenshot capture of quiz questions
- OCR text extraction with support for multiple languages (English, Azerbaijani, Russian)
- Image enhancement for better text recognition
- Integration with Google's Gemini AI for answer generation
- Simple keyboard controls

## Requirements

- Python 3.x
- Required Python packages:
  - easyocr
  - PIL (Pillow)
  - pyautogui
  - keyboard
  - requests
  - numpy

## Installation

1. Clone this repository:
```bash
git clone [repository-url]
cd QuizBot
```

2. Install the required packages:
```bash
pip install easyocr pillow pyautogui keyboard requests numpy
```

## Usage

1. Run the application:
```bash
python main.py
```

2. Controls:
   - Press 'j' to capture and process a screenshot
   - Press 'q' to exit the application

3. The application will:
   - Capture a screenshot of the specified region
   - Process the image to enhance text recognition
   - Extract text using OCR
   - Send the question to Gemini AI
   - Display the answer

## Configuration

The application uses the following default settings:
- Screenshot region: (150, 200, 800, 800)
- Supported languages: English and Azerbaijani (can be changed to Russian)
- Screenshots are saved in a 'screenshots' directory

## Notes

- Make sure you have a stable internet connection for the Gemini AI API to work
- The application requires appropriate permissions to capture screenshots
- Screenshots are automatically saved in the 'screenshots' directory with timestamps

## License

[Add your license information here]

## Disclaimer

This tool is intended for educational purposes only. Please use it responsibly and in accordance with your institution's policies regarding quiz-taking and academic integrity.
