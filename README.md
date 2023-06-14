## Chrome Passwords Extractor

This Python script allows you to extract saved passwords from the Google Chrome browser on Windows systems. It decrypts and retrieves the passwords stored in the Chrome database and saves them to a text file.

### Prerequisites

- Python 3.x
- Required Python packages: `base64`, `json`, `sqlite3`, `win32crypt` (Windows only), `Crypto.Cipher.AES`, `shutil`
- Google Chrome browser installed on the system

### Installation

1. Clone or download the script file to your local machine.

2. Install the required Python packages by running the following command in your terminal:
   ```
   pip install pycryptodomex pywin32
   ```

### Usage

1. Open a terminal or command prompt.

2. Navigate to the directory where you saved the script.

3. Run the script using the following command:
   ```
   python chromepasswords.py
   ```

4. The script will create a file named `chrome_passwords.txt` in the same directory. This file will contain the extracted Chrome passwords.

**Note:** The Chrome database file (`Login Data`) will be temporarily copied to the script's directory to avoid locking the original database file while Chrome is running. The copied file will be deleted after the extraction process.
