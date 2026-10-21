# Action Tracker

A small meeting action tracker for teams that keep forgetting what was agreed.

- Add an action with an owner and a due date
- Actions are grouped by owner, each with a tick box for done
- Open, done and overdue counts at the top, with overdue actions in red
- Light and dark themes follow the system setting

It is a single static page (`index.html`) with no build step and no dependencies. Fonts load from Google Fonts and fall back to system fonts.

## Data

Actions are saved in the browser's local storage, so each person sees only what was entered in their own browser. Clearing site data removes them. The first visit shows a few example actions, which can be removed with "Clear examples".

## Run locally

Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy to Vercel

1. In Vercel, choose **Add New → Project** and import this repository.
2. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
3. Click **Deploy**.

`vercel.json` enables clean URLs and adds basic security headers. Every push to `main` redeploys automatically.
