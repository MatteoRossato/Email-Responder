# Email Sender Project

This Python project allows you to send emails via an SMTP server with customizable credentials and settings.


## Features

- Send emails via SMTP.
- Support for sending emails with attachments.
- Configuration via a configuration file (`config.py`).
- Automated tests included to ensure correct functionality.

## Technologies

- Python 3.x
- Libraries:
  - `smtplib` (for sending emails)
  - `email.mime` (for managing attachments)
  - `unittest` (for automated tests)
- SMTP servers (e.g., Gmail, Outlook, etc.)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/email_sender_project.git
    cd email_sender_project
    ```

2. Create and activate a virtual environment (optional but recommended):

    ```bash
    python3 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

3. Install the project dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Configure the `config.py` file with your SMTP credentials and settings.

## Usage

To send an email, run the `email_sender.py` script or import the `send_email` function in your project.

### Example Usage:

```python
from email_sender import send_email

# Send email
send_email("subject", "body", "recipient@example.com")
