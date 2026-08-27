# FastAPI Project

A Python FastAPI backend project.

## Prerequisites

Make sure you have the following installed:

* Python 3.10+
* Git
* pip

## 1. Clone the Repository

```bash
git clone https://github.com/mayurpawar17/fastapi-demo.git
cd fastapi-demo
```

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

## 3. Install Dependencies

The project contains a `requirements.txt` file with the required Python packages.

```bash
pip install -r requirements.txt
```

## 4. Run the FastAPI Server

If your main FastAPI file is `main.py` and contains:

```python
app = FastAPI()
```

Run:

```bash
uvicorn main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

## 5. API Documentation

FastAPI automatically provides interactive API documentation.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

## 6. Project Setup for a New Developer

Every developer should create their **own virtual environment**.

Do not commit or share:

```text
venv/
__pycache__/
```

These are already included in `.gitignore`.

The required dependencies are stored in:

```text
requirements.txt
```

To recreate the environment:

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## 7. Updating Dependencies

When you install a new package:

```bash
pip install package-name
```

Update `requirements.txt`:

```bash
pip freeze > requirements.txt
```

Then commit the updated file:

```bash
git add requirements.txt
git commit -m "Update dependencies"
git push
```

## 8. Git Workflow

Before starting work:

```bash
git pull
```

After making changes:

```bash
git add .
git commit -m "Describe your changes"
git push
```

## Important

Do **not** commit:

```text
venv/
__pycache__/
.env
```

Do commit:

```text
requirements.txt
.gitignore
README.md
```
