# Sync GitHub Repository to AWS CodeCommit using GitHub Actions

## Setup

### Create CodeCommit Repository
- Go go AWS CodeCommit and create a repository

### Configuring OpenID Connect in AWS
We will use OpenID Connect within our workflow to authenticate with AWS. You can also use IAM user credentials for authentication.  
Please follow the below GitHub documentation create OIDC in AWS.  
- https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services
- https://www.automat-it.com/post/using-github-actions-with-aws-iam-roles

### Create GitHub Secrets
Create the following GitHub secrets
- `AWS_REGION` : region in which the CodeCommit repository is located
- `CODECOMMIT_REPOSITORY` : Codecommit repository name
- `CODECOMMIT_ROLE` : IAM role arn which was created in previous step

-- 