# Villa

## About the Project

Villa is a web application developed using Python and Django, with a website interface focused on villas and property-related content.

The application uses SQLite for database storage and Django for backend functionality. I included this project in my DevSecOps assignment to gain practical experience in applying security testing and automated deployment practices to a web application.

## Technologies Used

- **Python** – Programming language
- **Django** – Backend web framework
- **SQLite** – Database management
- **HTML, CSS and JavaScript** – Frontend development
- **Git and GitHub** – Source code management
- **Semgrep** – Static Application Security Testing (SAST)
- **Trivy** – Dependency vulnerability scanning
- **OWASP ZAP** – Dynamic Application Security Testing (DAST)
- **Jenkins** – CI/CD pipeline automation
- **Docker** – Application containerization
- **Amazon ECR** – Docker image storage
- **Kubernetes (K3s)** – Container orchestration
- **Argo CD** – GitOps-based deployment management

## Running the Application Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Afthabahammed/Villa.git
cd Villa
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Django

Set the required `DJANGO_SECRET_KEY` environment variable before running the application.

### 4. Apply Database Migrations

```bash
python manage.py migrate
```

### 5. Start the Development Server

```bash
python manage.py runserver
```

Open `http
