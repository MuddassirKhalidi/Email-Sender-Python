# Email With Python

This Python module provides a simple yet efficient way to send emails using SMTP (Simple Mail Transfer Protocol). Whether you need to send personalized emails to a group of recipients or a generic message to a single user, this module has got you covered.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Example](#example)
- [Requirements](#requirements)
- [Contributing](#contributing)

## Features

- Send emails to multiple recipients at once or individually.
- Personalize emails by addressing recipients by name.
- Support for sending emails via Gmail SMTP server.
- Easy-to-use interface for specifying email content and subject.

## Installation

1. Clone or download the repository to your local machine.
2. Ensure you have Python 3.x installed.
3. Install the required `smtplib` library.
   
```bash
pip install smtplib
```

## Usage

1. Import the `EmailSender` class into your Python script.
2. Create an instance of `EmailSender`.
3. Log in using your Gmail email address and App password.
4. Choose whether to send an email to one user or multiple users.
5. Follow the prompts to enter the subject and message content.
6. Email(s) will be sent accordingly.

## Example

```python
from email_with_python import EmailSender

# Create an instance of EmailSender
admin = EmailSender()

# Log in using your Gmail credentials
admin_email = admin.login()

# Choose whether to send an email to one user or multiple users
email_type = input('Email to one user [1] or to multiple [2]: ')
if email_type == '1':
    send_to_one_user()
else:
    send_email_to_group()

# Close the SMTP connection
admin.close_connection()
```

## Requirements

- Python 3.x
- `smtplib` library

## Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or create a pull request.
