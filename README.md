# CI-CD
CI/CD pipeline that detects which microservice changed in a monorepo push and builds only that service's Docker image, tags it with the commit SHA, and pushes to ECR. Jenkins/GitLab CI pipeline parses the git diff to identify changed paths, triggers targeted Docker builds, updates the Kubernetes deployment YAML with the new image tag, commits.
