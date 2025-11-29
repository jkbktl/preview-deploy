# Preview Deploy Test

Test repository for external contributor preview deployments.

## How it works

1. External contributor forks this repo and opens a PR
2. Maintainer reviews the code
3. Maintainer comments `/deploy` on the PR
4. GitHub Action builds and deploys to Vercel
5. Preview URL is posted as a comment

## Setup

Add these secrets to the repo (Settings → Secrets → Actions):

- `VERCEL_TOKEN` - Create at https://vercel.com/account/tokens
- `VERCEL_ORG_ID` - Your Vercel org/user ID
- `VERCEL_PROJECT_ID` - Your Vercel project ID

To get org/project IDs, run `vercel link` locally and check `.vercel/project.json`.
