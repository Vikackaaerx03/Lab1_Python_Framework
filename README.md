Password Security Lab | FastAPI Web Application
A robust, asynchronous web application designed to analyze and validate password strength based on modern security protocols. This project demonstrates the integration of a Python-based backend with a dynamic frontend using the FastAPI ecosystem.

Overview
The Password Lab is a security-focused tool that evaluates user input against five critical entropy criteria. It provides real-time feedback and actionable tips to help users create cryptographically strong passwords.

Core Validation Logic
The application enforces a strict security policy (Variant 11):

Length Constraint: Minimum of 12 characters.

Casing: Mandatory inclusion of both Uppercase (A-Z) and Lowercase (a-z) characters.

Numerical Density: Requires at least one digit (0-9).

Special Characters: Mandatory use of symbols (e.g., @, #, !, _, -) via RegEx validation.

Tech Stack
Backend: FastAPI (High-performance Python framework).

Templating: Jinja2 (Server-side rendering).

Frontend: HTML5 & CSS3 featuring a Glassmorphism UI design.

Server: Uvicorn (ASGI web server).

Environment Management: UV / Pip.

Project Architecture
The project follows a modular directory structure to ensure scalability and separation of concerns:

Plaintext
Lab1_Python_Framework/
├── app/
│   ├── routers/
│   │   └── password.py      # Core business logic & POST request handling
│   ├── static/
│   │   ├── photo_1.jpg      # High-definition vault background assets
│   │   └── style.css        # Global styles & responsive UI components
│   ├── templates/
│   │   ├── index.html       # Landing page (Main Entry Form)
│   │   └── result.html      # Dynamic Analysis Report page
│   └── main.py              # Application factory & router mounting
├── .gitignore               # Version control exclusion rules
├── pyproject.toml           # Project metadata & dependency locking
├── README.md                # Project documentation
└── uv.lock                  # Deterministic dependency resolution
Local Installation & Usage
1. Clone the Repository
Bash
git clone https://github.com/Vikackaaerx03/Lab1_Python_Framework.git
cd Lab1_Python_Framework
2. Environment Setup
Bash
# Create a virtual environment
python -m venv .venv

# Activate the environment
# For Windows:
.venv\Scripts\activate
# For Linux/macOS:
source .venv/bin/activate
3. Install Dependencies
Bash
pip install fastapi uvicorn jinja2 python-multipart
4. Launch the Application
Bash
uvicorn app.main:app --reload
The server will start at: http://127.0.0.1:8000

Author
Victoriia Roslav

Group: KN-732

University: National Technical University "Kharkiv Polytechnic Institute" (NTU "KhPI")

Faculty: Computer Science and Software Engineering