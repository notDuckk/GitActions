## CI/CD Workflow Documentation


This GitHub Actions workflow automates the building, testing, and deployment of a Node.js application to Heroku whenever code is pushed to the main branch.
Workflow Steps
1. Build Job

    Checkout Code: Retrieves the latest code from the repository.
    Install and Test: Installs dependencies and runs tests to ensure the application works correctly.

2. Deploy Job

    Setup Heroku CLI: Installs the Heroku command-line tool for deployment.
    Deploy: Pushes the application to Heroku, using an API key for authentication.

Configurations and Dependencies

    Node.js Version: The workflow uses Node.js version 14.
    Secrets: Requires the Heroku API key stored in GitHub secrets for secure access.