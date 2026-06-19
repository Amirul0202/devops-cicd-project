

## Project Overview
This project demonstrates a complete DevOps CI/CD workflow using GitHub Actions and AWS S3.

The application is a simple static website that is automatically built, tested, and deployed whenever changes are pushed to the repository.

---

## Technologies Used

- GitHub
- GitHub Actions
- Node.js
- Jest
- AWS S3
- MVisualStudios

---

## Project Structure

```text
devops-cicd-project/
│
├── index.html
├── style.css
├── script.js
├── package.json
├── tests/
│   └── app.test.js
│
├── .github/
│   └── workflows/
│       ├── build.yml
│       ├── test.yml
│       └── deploy.yml
│
└── README.md
```

---

## CI/CD Pipeline

### 1. Build Pipeline

The build pipeline:

- Checks out source code
- Installs dependencies
- Builds the application
- Uploads artifacts

### 2. Test Pipeline

The test pipeline:

- Runs unit tests using Jest
- Performs dependency scanning using npm audit
- Sends notification if tests fail

### 3. Deployment Pipeline

The deployment pipeline:

- Connects to AWS
- Uploads website files to S3 bucket
- Updates application version

---


## Pipeline Flow

```text
Code Push
    ↓
Build Pipeline
    ↓
Test Pipeline
    ↓
Deploy Pipeline
    ↓
AWS S3 Website
```

---

## Deployment

The website is automatically deployed to AWS S3 when all pipelines complete successfully.

Website URL:

(http://amirul-devops-site.s3-website-ap-southeast-2.amazonaws.com)

---

## Screenshots

### Build Pipeline
<img width="1920" height="1080" alt="Desktop Screenshot 2026 06 19 - 11 10 04 02" src="https://github.com/user-attachments/assets/2d93a428-80cd-4af0-9d64-ad98c37a9a15" />

### Test Pipeline
<img width="1920" height="1080" alt="Desktop Screenshot 2026 06 19 - 11 11 07 63" src="https://github.com/user-attachments/assets/4a16d095-be99-4dd1-8f6b-a7ad03f2ccd4" />

### Deployment Pipeline
<img width="1920" height="1080" alt="Desktop Screenshot 2026 06 19 - 11 11 17 80" src="https://github.com/user-attachments/assets/d10fc725-fe5c-48cc-b58f-53a2f8ef10d6" />

### AWS S3 Website
<img width="1920" height="1080" alt="Desktop Screenshot 2026 06 19 - 20 04 21 72" src="https://github.com/user-attachments/assets/f693a0c9-5844-444a-9cf1-a796f65373af" />

---

## Author

Name: Amirul Adha Bin Saifuzzaman

Course: BCF (Cloud Computing
