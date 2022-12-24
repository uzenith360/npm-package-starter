# NPM Package Starter
A TypeScript NPM starter (or example) project to ease setup of NPM packages from your GitHub repo

# Sources
[Andreybleme](https://andreybleme.com/2020-05-31/hosting-private-npm-packages-for-free/)  
[Snyk blog](https://snyk.io/blog/best-practices-create-modern-npm-package/)  
[Dev.to](https://dev.to/kouts/automated-versioning-and-package-publishing-using-github-actions-and-semantic-release-1kce)

# Secrets
For this setup you will need to create 3 auth tokens and save them as secrets in the github repo's settings, 
1. NPM token: An Automation-type access token from npm to be used solely in CI environments so that it is able to work around your account’s 2FA. To create one, go to https://www.npmjs.com/settings/\<your-npm-account\>/tokens. Be sure to select the type “Automation” as this will be used in a CI/CD workflow. i named it NPM_TOKEN
2. Github repo token: A personal access token from GitHub, to enable github actions access your public repositories. To create one go to https://github.com/\<your-name-or-github-organization\>/\<your-repo-name\>/settings/secrets/actions/new and select public_repo scope. I named it GH_Token
3. Synk API token: Snyk is a tool that simplifies security checks, to help monitor for, alert on, and offer assistance to mitigate vulnerabilities. Snyk is free, so sign-up and get your [Snyk API Token](https://app.snyk.io/account). Add your Snyk API Token as a Repository Secret on GitHub: https://github.com/\<your-account-or-organization\>/\<your-repo-name\>/settings/secrets/actions/new. I named it SNYK_TOKEN

Don't forget to search/replace my github handle and NPM Package name/Github repo with yours, after you fork/clone/download this repo :)

If you like it remember to **give repo a star**⭐