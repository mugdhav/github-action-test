# github-action-test
This repository contains an example Github Actions workflow, called GitHub Actions Assignment and defined using a .github/workflows/github-actions-demo.yml file.
The workflow contains a single job, called Assignment-GitHub-Actions. This job runs a few steps that echo information about:
- The event that triggers this job (push to this repository)
- The operating system this job runs on (ubuntu linux)
- The repository name and branch this job runs on
- And so on

This job checks out this repository's code to the job runner provided by GitHub, using the existing ***checkout*** action.
