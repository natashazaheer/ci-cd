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


Reference Articles Used

https://medium.com/@pathirage/step-in-to-ci-cd-a-hands-on-guide-to-building-ci-cd-pipeline-with-github-actions-7490d6f7d8ff

https://medium.com/@flymingotech/how-to-set-up-continuous-deployment-with-github-actions-2025-guide-e84aa6e379ac
