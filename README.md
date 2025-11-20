Emoji to Text Conversion Using demoji in Python

This project demonstrates how to convert emojis into their textual descriptions using the demoji Python library.

✨ Features

Detects emojis in a given text

Converts emojis to meaningful text labels

Works with multi-part emojis (e.g., 👨‍🎓, 👩‍🍳)

📦 Installation

Make sure you have Python 3 installed.

Install the required module:

pip install demoji


Download the latest emoji codes (required for first-time use):

import demoji
demoji.download_codes()

🧪 Example Usage
import demoji

text = "i am a former son 👨‍🎓.and my mother is housewife👩‍🍳"
result = demoji.findall(text)
print(result)

✅ Output
{
  '👨\u200d🎓': 'man student',
  '👩\u200d🍳': 'woman cook'
}


This output shows the detected emojis mapped to their textual descriptions.

📁 Project Structure
│── script.py
│── README.md

📝 Notes

demoji.download_codes() must be run once to download emoji metadata.

After downloading codes, the module will work offline.

The findall() method returns a dictionary of all emojis found in the given text.

🧑‍💻 Author

Your Name
Naga Amaresh Nuti
