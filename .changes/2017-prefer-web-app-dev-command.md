### Fixed

- **`@reticlehq/server` — `next_action` sent the agent to a backend or read-only folder.** When a project folder held a backend beside the web app, the no-session answer could hand the agent `npm run dev` for the backend. It now chooses only writable web apps, so the agent starts the app that serves the page. Closes [#2017](https://github.com/reticlehq/reticle/issues/2017).
