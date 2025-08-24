# Flask CI/CD with GitHub Actions

## Project Description
Simple Python Flask web application with automated CI/CD pipeline using GitHub Actions.

## Application
- Python Flask web app
- Shows a welcome page with server details
- Runs on port 5000

## CI/CD Pipelines

### CI Pipeline (main.yml)
- Triggers on push to main
- Installs dependencies
- Builds project  
- Uploads artifacts

### CD Pipeline (deploy.yml)  
- Uses self-hosted runner
- Downloads artifacts from CI
- Automatically runs after CI completes
- Deploys the Flask app

├── app.py                    # Main Flask application
├── requirements.txt          # Python dependencies
├── .github/workflows/
│   ├── main.yml             # CI Pipeline
│   └── deploy.yml           # CD Pipeline
└── README.md                # This file
