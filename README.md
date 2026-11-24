# Claude Agent Design Study Series

Interactive, mobile-friendly flashcard site for studying Claude agent design concepts.

**Current set:** Study Day 2 — Workflows vs Agents & Task Decomposition

Sources: Anthropic Building Effective Agents, Claude Cookbook (Basic Workflows), Claude Managed Agents Overview.

## Live site

To make this accessible on any device (including mobile):

1. Go to the repo **Settings** → **Pages**
2. Under **Build and deployment** → **Source**, select **Deploy from a branch**
3. Choose branch **main** / **/(root)**
4. Save

After a minute or two the site will be live at:

**https://swiftsolves-msft.github.io/claude-agent-study/**

Progress ("Known" cards) is stored in your browser's localStorage, so it persists on the same device.

## Features

- Tap/click card to flip
- Swipe left/right or use buttons to navigate
- Mark cards as known (progress saved locally)
- Day selector — ready for future study days
- Fully responsive / mobile-first

## Adding future study days

Edit `index.html` and add a new entry to the `studyData` object. Example:

```js
"3": {
  title: "Study Day 3: Your Topic Here",
  cards: [
    {
      front: "<h3>Question here</h3>",
      back: "<p>Answer here.</p>"
    }
    // more cards...
  ]
}
```

Then commit the change. The day selector will automatically pick it up.

## Local use

You can also open `index.html` directly in any browser (download from the repo or from Grok artifacts).
