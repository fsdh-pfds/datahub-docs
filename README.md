# FSDH Wiki & Help Guides

## Overview

This repository manages our FSDH wiki & help guides content and its deployment across multiple environments. Changes are developed in feature branches, reviewed via pull requests (PRs), and merged into the `main` branch. Our deployment process is automated for development and manually controlled for staging and production releases.

## Development Workflow

- **Branching & Pull Requests:**  
  Developers create feature branches and open PRs for their changes. Code is reviewed and approved before being merged into the `main` branch.

- **Automatic Development Deployment:**  
  When a PR is merged into `main`, the latest changes are automatically deployed to our **development** environment. This ensures that the current state of the project is immediately available in a live setting for further testing and feedback.

## Release Process

- **Staging (Pre-production):**  
  Releases to staging are manually triggered. A dedicated workflow deploys the content to our staging environment, where further testing and validation occur.

- **Production:**  
  Once the staging release has been reviewed and validated, a separate manual trigger promotes the release to our **production** environment. Production releases require an additional review step to ensure stability before going live.


## Summary

- **Changes Flow:**  
  1. Develop in feature branches.
  2. Merge changes into `main` via a pull request requiring a human review.
  3. Automatic deployment to development on merge.
  
- **Releases:**  
  - **Staging and Production:** Both are triggered manually, with review steps at each stage to ensure only verified changes are promoted to these environments.

This process balances rapid development feedback (via automatic dev deployments) with careful control over live production updates, ensuring quality and stability throughout the release cycle.
