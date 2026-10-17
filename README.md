# DevOps Status Dashboard 

A simple web application built with **Python and Flask** as the starting point for an end-to-end DevOps project.

##  Technologies Used

* Python
* Flask
* HTML/CSS
* Git
* GitHub

##  Project Structure

```text
devops-status-dashboard/
│
├── app/
│   ├── app.py
│   ├── requirements.txt
│   └── templates/
│       └── index.html
│
├── .gitignore
└── README.md
```

##  Setup and Run

### 1. Clone the repository

```bash
git clone <repository-url>
cd devops-status-dashboard
```

### 2. Create a virtual environment

```bash
py -m venv venv
```

### 3. Activate the virtual environment

On Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```powershell
pip install -r app\requirements.txt
```

### 5. Run the application

```powershell
py app\app.py
```

The application will be available at:

```text
http://localhost:5000
```

##  Health Check

A health-check endpoint is available at:

```text
http://localhost:5000/health
```

Example response:

```json
{
    "application": "DevOps Status Dashboard",
    "status": "healthy",
    "version": "1.0"
}
```
