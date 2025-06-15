# Daily Journal Web Application

This project is a full-stack web application that allows users to maintain a daily journal.

## Project Overview

The Daily Journal Web Application enables users to:
- View an inspiring daily quote
- Submit journal entries about their feelings and experiences
- View their past journal entries
- Track their emotional journey over time

## Tech Stack

| Layer             | Technology                         |
|-------------------|------------------------------------|
| **Frontend**      | HTML + CSS + JavaScript (or React) |
| **Backend**       | Python + Flask                     |
| **Database**      | SQLite                             |
| **Version Control** | Git + GitHub                       |
| **IDE**           | VS Code                            |

## Getting Started

### Prerequisites
- Install [VS Code](https://code.visualstudio.com/)
- Install [Python 3.8+](https://python.org/downloads/)
- Install [Git](https://git-scm.com/downloads)
- Create a [GitHub account](https://github.com/)

### Project Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/daily-journal.git
    cd daily-journal
    ```

2.  **Project Structure:**
    ```
    daily-journal/
    ├── backend/
    │   ├── app.py
    │   ├── database.py
    │   ├── models.py
    │   └── requirements.txt
    ├── frontend/
    │   ├── index.html
    │   ├── style.css
    │   ├── script.js
    │   └── assets/
    ├── README.md
    └── .gitignore
    ```

3.  **Backend Setup:**
    ```bash
    cd backend
    python -m venv venv

    # Activate virtual environment
    # Windows:
    venv\Scripts\activate
    # macOS/Linux:
    source venv/bin/activate

    # Install dependencies
    pip install flask flask-cors sqlite3
    pip freeze > requirements.txt
    ```

For more detailed instructions, please refer to `daily-journal-onboarding-task.md`.
