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

Open `http://127.0.0.1:8000` in your browser.

## DevSecOps Implementation

I integrated Villa into an automated DevSecOps workflow to practise security scanning, continuous integration, containerization, and deployment.

The workflow consists of the following stages:

1. **GitHub:** Stores the application source code.
2. **Semgrep:** Performs Static Application Security Testing (SAST).
3. **Trivy:** Scans project dependencies for known vulnerabilities.
4. **Jenkins:** Automates the CI/CD pipeline.
5. **Docker:** Packages the application into a container image.
6. **Amazon ECR:** Stores the Docker image.
7. **Kubernetes:** Deploys and manages the application.
8. **Argo CD:** Synchronizes deployment configurations through GitOps.
9. **OWASP ZAP:** Performs Dynamic Application Security Testing (DAST) on the running application.

## Deployment

The application is containerized using Docker and deployed on a Kubernetes cluster. Its Docker image is stored in Amazon ECR.

Argo CD manages the Kubernetes deployment by monitoring the separate GitOps repository and synchronizing the deployment configurations.

## Project Goal

The goal of this work was to understand how security testing, CI/CD automation, containerization, cloud image storage, Kubernetes, and GitOps can be combined to build a practical DevSecOps workflow.
