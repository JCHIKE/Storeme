# Storeme
# Secure Information Vault

## Project Overview
Secure Information Vault is a web application that enables users to securely store and retrieve vital personal information. The data is encrypted and accessible only to the user, ensuring privacy and security.

## Tech Stack
- *Backend:* Python (Flask/Django)
- *Frontend:* HTML, CSS, JavaScript
- *Database:* PostgreSQL
- *Security Features:* AES Encryption, User Authentication, Two-Factor Authentication (2FA)

## Features
- *User Authentication*: Secure login system with password hashing.
- *Data Encryption*: AES encryption ensures stored information remains private.
- *Secure Data Storage*: Uses PostgreSQL to store user data securely.
- *Access Control*: Users can retrieve stored data only after authentication.
- *Two-Factor Authentication (2FA)*: Adds an extra layer of security.
- *Backup & Recovery*: Users can backup encrypted data and restore when needed.
- *Session Management*: Auto logout after inactivity.

## Installation
### Prerequisites
Ensure you have the following installed on your system:
- Python 3.9+
- PostgreSQL
- Virtual Environment (venv)

### Setup Instructions
1. *Clone the repository:*
   sh
   git clone https://github.com/yourusername/secure-info-vault.git
   cd secure-info-vault
   
2. *Create and activate a virtual environment:*
   sh
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   
3. *Install dependencies:*
   sh
   pip install -r requirements.txt
   
4. *Configure the database:*
   - Create a PostgreSQL database.
   - Update the .env file with database credentials.

5. *Run migrations:*
   sh
   python manage.py migrate  # If using Django
   

6. *Start the application:*
   sh
   python manage.py runserver  # If using Django
   
   Or for Flask:
   sh
   flask run
   

## Usage
1. Register a new account.
2. Log in to access the secure vault.
3. Add, retrieve, or delete stored information.
4. Use 2FA for enhanced security.

## Security Measures
- *AES Encryption*: Ensures sensitive data is encrypted before storage.
- *Hashed Passwords*: Uses bcrypt for password security.
- *Role-Based Access Control*: Limits access based on user privileges.
- *Auto Logout*: Protects against unauthorized access.

## Future Enhancements
- Mobile app integration.
- Multi-device sync.
- Biometric authentication.

## License
This project is licensed under the MIT License.