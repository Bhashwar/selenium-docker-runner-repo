# Selenium Docker Runner

This repository contains Docker Compose and Jenkinsfile definitions for running Selenium-based tests in a grid setup. The grid includes:
- A Selenium Hub (`selenium/hub`)
- Chrome and Firefox nodes
- Two test services (`vendor-portal` and `flight-reservation`) that pull from `neel2025/selenium`.

## Files

- **docker-compose.yml**  
  Defines services for
    - `AutomationHub` (Selenium Hub)
    - `chrome` and `firefox` (browser nodes)
    - `vendor-portal` and `flight-reservation` (test containers)

- **Jenkinsfile**  
  A Jenkins Pipeline that can start and stop these services and run tests.

## Usage

1. **Clone the repo**:
   ```bash
   git clone https://github.com/Bhashwar/selenium-docker-runner-repo.git
