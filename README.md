  📱 WhatsApp Web Automation with Selenium (Python)
  
This project automates WhatsApp Web using Python and Selenium to send a text message and an image/file to multiple phone numbers stored in a CSV file.
⚠️ Disclaimer: This project is for educational purposes only. Automating WhatsApp may violate WhatsApp’s Terms of Service. Use responsibly.

✨ Features
📄 Read phone numbers from a CSV file
💬 Send an automated text message
📎 Attach and send an image or any file
🖱 Click the Send button programmatically
🔁 Loop through multiple contacts automatically
⏳ Smart waits for stable execution

🛠 Tech Stack
Python 3.8+
Selenium
webdriver-manager
Pandas
Google Chrome

📂 Project Structure
whatsapp-web-automation/
│
├── numbers.csv
├── send_whatsapp_file.py
├── README.md

📄 CSV File Format

The CSV file must contain a column named phone.

Example: numbers.csv
phone
918269596909
916265800597
918226021374


📌 Phone numbers must include country code
📌 Do NOT include +, spaces, or special characters

⚙️ Configuration

Edit the following variables inside the script:

FILE_PATH = "numbers.csv"
MESSAGE = "hyy"
FILE_TO_SEND = r"C:\Users\YourName\Pictures\image.png"

Variable	Description
FILE_PATH	Path to CSV file
MESSAGE	Text message to send
FILE_TO_SEND	Absolute path of the file/image
📦 Installation
1️⃣ Install Dependencies
pip install selenium webdriver-manager pandas

2️⃣ Install Google Chrome

Make sure Google Chrome is installed and updated.

▶️ How to Run the Script
python send_whatsapp_file.py

First Run Instructions:
Chrome will open WhatsApp Web
Scan the QR code using your phone
Script starts automatically after login

🔄 How the Script Works
Step 1: Open WhatsApp Web

Launches Chrome browser
Waits for QR code login

Step 2: Open New Chat

Clicks the New Chat icon

Step 3: Search Phone Number

Types the phone number

Presses ENTER to open the chat

Step 4: Send Text Message

Types the predefined message

Sends it using ENTER key

Step 5: Attach File

Clicks the attachment (📎) icon

Selects the file using file input

Step 6: Click Send Button

Waits for the media preview

Clicks the Send button using XPath

Step 7: Repeat

Loops through all phone numbers in the CSV file

🛡 Safety Guidelines

⚠️ Important Recommendations

Keep a delay of 8–10 seconds between messages

Avoid sending messages to unknown numbers

Do not send large volumes at once

Excessive automation may lead to temporary account bans

❗ Common Issues & Solutions
Issue	Solution
File not sending	Increase wait time before clicking send
XPath not found	WhatsApp UI may have changed
QR appears repeatedly	Clear browser cache
Message not delivered	Check phone number format
⚠ Limitations
Relies on WhatsApp Web UI (XPaths may break)
Manual QR code scanning required
Not designed for high-volume spam messaging

🚀 Future Improvements

✅ Retry failed numbers
📊 Excel file support
🖼 Add captions to images
📁 Multiple file support
📈 Message status logging
⚖ Legal Notice

This project is intended only for learning and testing.

👨‍💻 Author
Aman Rajput
Python Automation Developer
