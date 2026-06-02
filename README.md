# GitHub Repository Access Tracker

A Bash automation script that uses the GitHub REST API to list repository collaborators with read access. The script authenticates using a GitHub Personal Access Token (PAT) and displays collaborator usernames and GitHub user IDs.

## Features

* Retrieve repository collaborators using the GitHub API
* Filter users with read (pull) access
* Display GitHub usernames and user IDs
* Argument validation for repository owner and repository name
* Debugging and error handling support

## Prerequisites

Before running the script, ensure the following tools are installed:

* Bash
* curl
* jq
* GitHub Personal Access Token (PAT)

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/GitHub-Repository-Access-Tracker.git
cd GitHub-Repository-Access-Tracker
```

### 2. Export GitHub Credentials

```bash
export username="your_github_username"
export token="your_github_personal_access_token"
```

### 3. Make the Script Executable

```bash
chmod +x github_access_tracker.sh
```

## Usage

```bash
./github_access_tracker.sh <repo_owner> <repo_name>
```

### Example

```bash
./github_access_tracker.sh octocat Hello-World
```

### Sample Output

```text
Listing users with read access to octocat/Hello-World...

Username: octocat | ID: 583231
Username: user1   | ID: 12345678
Username: user2   | ID: 87654321
```

## Project Structure

```text
.
├── github_access_tracker.sh
└── README.md
```

## Technologies Used

* Bash Scripting
* GitHub REST API
* curl
* jq

## Learning Objectives

This project demonstrates:

* Bash scripting fundamentals
* Working with REST APIs
* GitHub API authentication
* JSON parsing using jq
* DevOps automation practices
* Error handling and argument validation

## Author

Gugan

## License

This project is open source and available under the MIT License.
