Steps to Create a Token:
Go to GitHub Settings

1. Log in to your GitHub account.
  - Click on your profile picture in the top-right corner and select Settings
    
2. Access Developer Settings
  - Scroll down in the left sidebar and click on Developer settings.

3. Navigate to Personal Access Tokens
  - Under Developer settings, select Personal access tokens > Tokens (classic).

4. Generate a New Token
  - Click on Generate new token > Generate new token (classic).

5. Configure the Token
  - Provide a note to describe the token's purpose (e.g., "GitHub Actions Token").
  - Set an expiration date (optional but recommended for security).
  - Select the scopes for the token based on your needs:
  - repo: Full control of private repositories (required for private repo workflows).
  - workflow: Access to GitHub Actions workflows.

6. Generate and Save the Token
  - Click Generate token.
  - Copy the token immediately. You won’t be able to see it again.

7. Add the Token to GitHub Actions Secrets
  - Navigate to the repository where you want to use the token.
  - Go to Settings > Secrets and variables > Actions.
  - Click New repository secret.
  - Name it (e.g., PERSONAL_ACCESS_TOKEN) and paste the token into the value field ie. in `.yml` file
  - Save the secret.
