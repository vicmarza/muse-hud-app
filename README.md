# muse-hud-app

Built copies of Muse HUD (a MentraOS miniapp that shows Meta Muse replies on
Even Realities G1 glasses), Muse Bridge (the Android helper that reads Muse's
replies off its screen) and Claude HUD (a MentraOS miniapp that shows answers
and insights from Claude, using the live conversation). This repo holds only
the compiled apps, served by GitHub Pages so the phone can install them
without a computer.

## Install

1. **Muse Bridge:** on the phone, open
   <https://vicmarza.github.io/muse-hud-app/muse-bridge.apk>, install it,
   open it, turn it on in accessibility settings, and allow notifications.
2. **Muse HUD:** in the Mentra app, **Settings → Miniapp Developer Settings →
   Load Miniapp from URL**, then enter:

   ```
   https://vicmarza.github.io/muse-hud-app/
   ```

3. **Claude HUD:** the same way, with:

   ```
   https://vicmarza.github.io/muse-hud-app/claude-hud/
   ```

   Then open it and paste your Claude API key under **Start here**.

## Updating

Muse HUD's files (at the root) and Claude HUD's (in `claude-hud/`) come from
`bun run site` in each miniapp's folder of the source project, and
`muse-bridge.apk` from its GitHub Actions build. Replace them here and push to
`main`; Pages redeploys on its own.
