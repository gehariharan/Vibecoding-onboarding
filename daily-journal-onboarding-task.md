# 📔 Daily Journal - Full Stack Development Onboarding Task

Welcome to your first full-stack web development project! This task will help you learn the fundamentals of web development while building a practical daily journal application.

## 🎯 Project Overview

You'll be building a **Daily Journal Web Application** that allows users to:
- View an inspiring daily quote
- Submit journal entries about their feelings and experiences
- View their past journal entries
- Track their emotional journey over time

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Frontend** | HTML + CSS + JavaScript (or React) | User interface and interactions |
| **Backend** | Python + Flask | Server-side logic and API |
| **Database** | SQLite | Data storage |
| **Version Control** | Git + GitHub | Code management |
| **IDE** | VS Code | Development environment | Use any vibe coding IDE in free tier - WindSurf/Cursor
| **Deployment** | Vercel/AWS Amplify (Stretch Goal) | Hosting |

## 📋 Requirements

### Core Features (Must Have)
1. **Daily Quote Display** - GET request to show inspirational quotes
2. **Journal Entry Submission** - POST request to save user feelings/thoughts
3. **Entry History** - Display past journal entries
4. **Simple, clean UI** - User-friendly interface

### Stretch Goals (Nice to Have)
1. **Deployment** - Host on Vercel or AWS Amplify . For Backend You can host in render free tier. Stretch deploy this on a VM in AWS (Free Tier only)
2. **Enhanced UI** - Better styling and responsive design
3. **Entry Search** - Search through past entries
4. **Mood Tracking** - Visual representation of mood over time

## 🚀 Getting Started

### Prerequisites
- [ ] Install [VS Code](https://code.visualstudio.com/)
- [ ] Install [Python 3.8+](https://python.org/downloads/)
- [ ] Install [Git](https://git-scm.com/downloads)
- [ ] Create a [GitHub account](https://github.com/)

### Project Setup

1. **Create a new repository on GitHub**
   ```bash
   # On GitHub, create a new repository named "daily-journal"
   # Clone it to your local machine
   git clone https://github.com/yourusername/daily-journal.git
   cd daily-journal
   ```

2. **Set up project structure**
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

3. **Backend Setup**
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

## 💻 Development Guide

### Backend Development (Flask + SQLite)

**Key Components:**
- **Flask App** (`app.py`) - Main server application
- **Database** (`database.py`) - SQLite database setup and operations
- **Models** (`models.py`) - Data structures for journal entries

**API Endpoints to Implement:**
- `GET /api/quote` - Returns daily inspirational quote
- `POST /api/journal` - Saves a new journal entry
- `GET /api/journal` - Returns all journal entries
- `GET /api/journal/<date>` - Returns entries for specific date

### Frontend Development

**Key Files:**
- **HTML** (`index.html`) - Page structure and layout
- **CSS** (`style.css`) - Styling and responsive design
- **JavaScript** (`script.js`) - API calls and user interactions

**Features to Implement:**
- Daily quote display section
- Journal entry form (date, mood, text)
- Past entries display with date filtering
- Simple, clean design

### Database Schema

```sql
CREATE TABLE journal_entries (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    date DATE NOT NULL,
    mood VARCHAR(20),
    entry TEXT NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## 📝 Step-by-Step Plan

### Phase 1: Backend Foundation (Days 1-2)
- [ ] Set up Flask application
- [ ] Create SQLite database and tables
- [ ] Implement basic API endpoints
- [ ] Test API with Postman or curl

### Phase 2: Frontend Basics (Days 3-4)
- [ ] Create HTML structure
- [ ] Add CSS styling
- [ ] Implement JavaScript for API calls
- [ ] Test frontend-backend integration

### Phase 3: Features & Polish (Days 5-6)
- [ ] Add journal entry form
- [ ] Display past entries
- [ ] Implement daily quote feature
- [ ] Improve UI/UX

### Phase 4: Deployment (Day 7 - Stretch Goal)
- [ ] Deploy backend to a hosting service
- [ ] Deploy frontend to Vercel/Netlify
- [ ] Test production deployment
- [ ] Share live URL

## 🔧 Useful Resources

### Documentation
- [Flask Documentation](https://flask.palletsprojects.com/)
- [SQLite Tutorial](https://www.sqlitetutorial.net/)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Git Tutorial](https://git-scm.com/docs/gittutorial)

### Free APIs for Quotes
- [Quotable API](https://github.com/lukePeavey/quotable)
- [Zen Quotes API](https://zenquotes.io/)
- [Quote Garden API](https://pprathameshmore.github.io/QuoteGarden/)

### Deployment Platforms
- [Vercel](https://vercel.com/) - Frontend hosting
- [Railway](https://railway.app/) - Backend hosting
- [AWS Amplify](https://aws.amazon.com/amplify/) - Full-stack hosting

## 🧪 Testing Your Application

Ensuring your application works as expected is crucial. Testing helps catch bugs early and maintain code quality.

### Types of Testing
- **Unit Testing**: Test individual functions or components in isolation.
    - **Backend (Python/Flask)**: Use libraries like `pytest` or Python's built-in `unittest` module to test your API endpoints, database functions, and business logic.
    - **Frontend (JavaScript/React)**: Use frameworks like Jest, Mocha, or Jasmine to test individual UI components and functions.
- **Integration Testing**: Test the interaction between different parts of your application, such as the frontend and backend, or your application and the database.
- **End-to-End (E2E) Testing**: Simulate real user scenarios by testing the entire application flow from the user interface to the backend and database. Tools like Selenium, Cypress, or Playwright can be used for E2E testing.Use things of your choice

### Suggested Tools
- **Pytest**: A popular testing framework for Python that makes it easy to write small, readable tests.
- **Jest**: A delightful JavaScript Testing Framework with a focus on simplicity. Often used with React.
- **Mocha**: A feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun.
- **Postman/Insomnia**: Useful for manually testing your API endpoints during development.

### Best Practices for Testing
- Write tests for new features as you develop them.
- Aim for good test coverage, especially for critical parts of your application.
- Run tests frequently, especially before committing code.
- Keep your tests independent and repeatable.

## 📊 Evaluation Criteria

### Technical Skills (60%)
- [ ] Working Flask backend with proper API endpoints
- [ ] Functional SQLite database integration
- [ ] Clean, responsive frontend
- [ ] Proper error handling
- [ ] Code organization and structure

### Best Practices (25%)
- [ ] Proper Git workflow with meaningful commits
- [ ] Clear code comments and documentation
- [ ] Appropriate project structure
- [ ] Requirements.txt and dependency management

### Creativity & Polish (15%)
- [ ] UI/UX design quality
- [ ] Additional features beyond requirements
- [ ] Deployment (if attempted)
- [ ] Overall user experience

## 🚀 Submission Guidelines

### Required Deliverables
1. **GitHub Repository** with complete source code
2. **README.md** with setup instructions
3. **Working application** (locally or deployed)

### Submission Format
- **GitHub Repository URL**: `https://github.com/yourusername/daily-journal`
- **Live Demo URL** (if deployed): `https://your-app.vercel.app`
- **Setup Instructions**: Include in your README

### Git Best Practices
```bash
# Make frequent, meaningful commits
git add .
git commit -m "Add journal entry form with validation"
git push origin main

# Use branches for features
git checkout -b feature/quote-api
git checkout -b feature/entry-history
```

## 💡 Pro Tips

1. **Start Simple** - Get basic functionality working before adding features
2. **Test Early** - Test your API endpoints as you build them
3. **Commit Often** - Make small, frequent commits with clear messages
4. **Use AI to refine** - Don't hesitate to use any AI tools of choice to refine your code (stick to free version for now)
5. **Document Everything** - Write clear README and code comments
6. **Plan Your UI** - Sketch your interface before coding

## 🎉 Success Metrics

By the end of this project, you should be able to:
- ✅ Build a complete full-stack web application
- ✅ Work with databases and APIs
- ✅ Use Git for version control effectively
- ✅ Deploy applications to the cloud
- ✅ Write clean, maintainable code
- ✅ Debug and troubleshoot issues independently

---

**Good luck with your first full-stack project! Remember, the goal is to learn and have fun building something useful. Don't worry about making it perfect – focus on making it work first! 🚀**

---

