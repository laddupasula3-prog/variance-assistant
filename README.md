# Variance Assistant

Claude-powered budget vs actual commentary. Variances are computed in code, Claude drafts the narrative, and a validation step checks every number in the output against the input data.

Includes a Claude Skill: `skills/variance-commentary/SKILL.md`.

## Run locally
```
npm install
cp .env.example .env.local   # add your ANTHROPIC_API_KEY
npm run dev
```

## Deploy (GitHub + Vercel)
1. Create a GitHub repo and push this folder to `main`.
2. Go to vercel.com, sign in with GitHub, click Add New > Project, and import the repo.
3. Under Environment Variables, add `ANTHROPIC_API_KEY`. Click Deploy.
4. Vercel gives you a URL like `https://your-project.vercel.app`. Every push to `main` redeploys; pull requests get preview URLs.
5. Put the Vercel URL and the GitHub repo link in your application.
