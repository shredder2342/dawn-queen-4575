# Next.js Framework Starter

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/cloudflare/templates/tree/main/dawn-queen-4575)

<!-- dash-content-start -->

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app). It's deployed on Cloudflare Workers as a [static website](https://developers.cloudflare.com/workers/static-assets/).

<!-- dash-content-end -->

Outside of this repo, you can start a new project with this template using [C3](https://developers.cloudflare.com/pages/get-started/c3/) (the `create-cloudflare` CLI):

```bash
npm create cloudflare@latest -- --template=cloudflare/templates/dawn-queen-4575
```

A live public deployment of this template is available at [https://dawn-queen-4575.templates.workers.dev](https://dawn-queen-4575.templates.workers.dev)

## Getting Started

First, run:

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

Then run the development server (using the package manager of your choice):

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Deploying To Production

| Command           | Action                                       |
| :---------------- | :------------------------------------------- |
| `npm run build`   | Build your production site                   |
| `npm run preview` | Preview your build locally, before deploying |
| `npm run deploy`  | Deploy your production site to Cloudflare    |

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## n8n Workflow

A ready-to-import workflow is available at `n8n/workflows/scrape-latest-article.json`. It uses a Telegram bot to receive a message containing a website URL, scrapes the latest article on that site, summarizes it with the OpenAI node and sends the result back to Telegram.

1. Import the JSON file in your n8n instance.
2. Configure credentials for **Telegram** and **OpenAI**.
3. Start the workflow and send a site URL (for example `https://www.goldmansachs.com/insights/`) to your bot.

The workflow will respond with a short summary of the article's main points.

