# NPM Package Starter

A TypeScript NPM starter (or example) project to ease setup of NPM packages from your GitHub repo

## Setup

1. git clone https://github.com/uzenith360/npm-package-starter
2. npm install
3. Search/replace my github handle and NPM Package name/Github repo with yours
4. Create github/NPM/Synk auth tokens (See secrets section below) and add to the secrets in your github repo

## Secrets

For this setup you will need to create 3 auth tokens and save them as secrets in your github repo's settings, 
1. NPM token: An Automation-type access token from npm to be used solely in CI environments so that it is able to work around your account’s 2FA. To create one, go to https://www.npmjs.com/settings/<your-npm-account\>/tokens. Be sure to select the type “Automation” as this will be used in a CI/CD workflow. i named it NPM_TOKEN
2. Github repo token: A personal access token from GitHub, to enable github actions access your public repositories. To create one go to https://github.com/settings/tokens select Personal access tokens > Tokens (Classic). Click on the button to create new token and select repo (Full control of private repositories), write:packages and delete:packages. I named it GH_Token
3. Synk API token: Snyk is a tool that simplifies security checks, to help monitor for, alert on, and offer assistance to mitigate vulnerabilities. Snyk is free, so sign-up and get your [Snyk API Token](https://app.snyk.io/account). Add your Snyk API Token as a Repository Secret on GitHub: https://github.com/<your-account-or-organization\>/\<your-repo-name\>/settings/secrets/actions/new. I named it SNYK_TOKEN

## Sources

I would like to acknowledge the authors of these blogs for providing helpful content on the topic, I encourage you to read too :)
- [Andreybleme](https://andreybleme.com/2020-05-31/hosting-private-npm-packages-for-free/)  
- [Brian Clark on Snyk blog](https://snyk.io/blog/best-practices-create-modern-npm-package/)  
- [Giannis Koutsaftakis on Dev.to](https://dev.to/kouts/automated-versioning-and-package-publishing-using-github-actions-and-semantic-release-1kce)

## Support

For support, open an issue or email wogwugwu.zenith@gmail.com, I will do my best to respond to all issues

## Important

Don't forget to search/replace my github handle and NPM Package name/Github repo with yours, after you fork/clone/download this repo :)



