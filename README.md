# SkillTrackr

SkillTrackr is a collaborative web project built using modern frontend tools.  
This repository is open for contributions and follows a clean Git workflow to keep the code stable and organized.

---

## 🛠 Tech Stack

- **Backend:** Django, Python  
- **Frontend:** HTML, Tailwind CSS  
- **Database:** SQLite (default)  
- **Version Control:** Git  
- **Package Managers:** pip, npm  

---

## 📖 Getting Started

Follow the steps below after cloning the repository.

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/skilltrackr.git
cd skilltrackr
```
### 2. Create and Activate Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate
```
For Windows:
```bash
venv\Scripts\activate
```
### 3. Install Python Dependencies
```bash
pip install -r requirements.txt
```
### 4. Install Node Dependencies
Make sure Node.js is installed on your system.
```bash
npm install
```
### 5. Build Tailwind CSS
Run the Tailwind build command:
```bash
npx tailwindcss -i ./static/src/input.css -o ./static/dist/output.css --watch
```
> Keep this command running in a separate terminal while developing frontend styles.

### 6. Apply Database Migrations
```bash
python manage.py migrate
```
### 7. Run the Development Server
```bash
python manage.py runserver
```
Open the application in the browser:
http://127.0.0.1:8000/

## 🔄 Development Workflow

### Branch Strategy (Very Important)

We follow this branching model:

- **main** → Stable / production-ready code (protected)  
- **dev** → Active development branch  
- **feature/*** → Individual feature branches  

### Workflow
feature/* → dev → main

### Rules
- ❌ Do **NOT** push directly to `main`  
- ❌ Do **NOT** push directly to `dev`  
- ✅ Always create a `feature/*` branch  
- ✅ Raise a Pull Request to `dev`  

> Only the repository owner merges `dev` → `main`.

### Create a New Feature Branch

```bash
git checkout dev
git pull origin dev
git checkout -b feature/your-feature-name
```
### Commit Changes

```bash
git add .
git commit -m "Meaningful commit message"
```
### Push Feature Branch

```bash
git push origin feature/your-feature-name
```
### Merge into Dev Branch
- Create a Pull Request from feature/your-feature-name → dev
- Review and merge the changes
- Delete the feature branch after merge

## Branch Cleanup (After Merge)

### Delete local branch:

```bash
git branch -d feature/your-feature-name
```

### Delete remote branch:

```bash
git push origin --delete feature/your-feature-name
```