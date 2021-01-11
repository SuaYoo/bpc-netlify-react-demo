# BPC Netlify + React demo

React app for Netlify demo

[Live demo: https://bpc-netlify-react-demo.netlify.app](https://bpc-netlify-react-demo.netlify.app/)

## 1. Set up GitHub project

### Option 1: Clone this repo

1. Clone this repo: `git clone git@github.com:SuaYoo/bpc-netlify-react-demo.git` (or use git client)
2. Reset your git history to the first commit: `git reset --hard 08c4560772d15f58c00377ab536b73a7d373f274`

### Option 2: Create new repo

1. Create a new public GitHub repo
2. Clone your new repo and go to the repo directory in your terminal (or git client)
3. Run `npx create-react-app .`
4. Commit any changes and push

## 2. Set up Netlify project

1. [Sign up with Netlify](https://app.netlify.com/signup) (Using GitHub preferred)
2. [Create a new site](https://app.netlify.com/start)
3. Click **GitHub** under **Continuous Deployment** and authorize Netlify in popup
4. Click **Configure Netlify on GitHub** and complete configuration
5. Go back to Netlify new site view, choose your demo repo from the list
6. Confirm or update the default settings for **Basic build settings**:
   - Build command: **npm run build**
   - Publish directory: **build/**
7. Click **Deploy site**
8. Go to **Site settings** and **Change site name**
9. Go to **Deploys**
10. If you see "**Production**: main@`HEAD` Published", visit your site URL to see it live. If you see "Building", wait for the deploy to finish and then visit your site

## 3. Update your app

1. Make some changes to the `App` component in `src` ([Example commit](https://github.com/SuaYoo/bpc-netlify-react-demo/commit/10b0616463eeaaae697b4c12210776ab0ed828a8))
2. Test that your changes build locally by running `npm run build`
3. If build succeeds, commit and push your changes to the `main` branch
4. Go to back to your Netlify dashboard. Monitor the new deploy, and verify your changes in production once live

For more instructions on running the actual React app, see [CRA](./CRA.md)
