# Ember

A dark, fast Discord theme for [Vencord](https://vencord.dev) and BetterDiscord, with warm clay accents inspired by Claude's colour palette.

## What it focuses on

- **Performance first.** No animations, no transitions, no backdrop blur, no web fonts and no remote `@import`. The whole theme is one local file, so nothing downloads when Discord starts. Message and member rows are isolated with CSS `contain` so new embeds or reactions don't relayout the whole list.
- **Less clutter.** Hides Nitro, Shop and Quests, gift / GIF / sticker / Apps buttons in the chat bar, the member list Activity section, activity cards, the Discover and Download buttons, avatar decorations, nameplates and profile effects.
- **A darker look.** Near-black charcoal panels floating on a softly lit background, cream text and clay-orange accents on links, buttons, the selected channel and the focused message box.
- **Fully configurable.** Every colour, spacing value, font and feature has a switch in the config block at the top of the file.

## Install

1. Download [`ember.theme.css`](ember.theme.css).
2. **Vencord:** Settings → Themes → Open Themes Folder, drop the file in, then enable **Ember**.
   **BetterDiscord:** put it in your BetterDiscord `themes` folder and enable it.
3. Optional: set Discord's Settings → Accessibility → Reduced Motion to on.

## Customise

Open the file and edit the `CONFIG` block at the top. A few examples:

| Setting | Default | What it does |
| --- | --- | --- |
| `--chat-width` | `1040px` | Centred reading column. `none` = full width |
| `--gap` | `10px` | Space between panels |
| `--animations` | `off` | Turn Discord's animations back on |
| `--hide-nitro` / `--hide-activity` / `--hide-chat-buttons` / `--hide-decorations` | `on` | Debloat groups |
| `--canvas-glow` | `on` | Static clay glow behind the panels |
| `--font` | `'Segoe UI Variable Text'` | `''` for Discord's default font |

Colours live in `:root` right below: `--bg-1` to `--bg-4` for surfaces, `--text-1` to `--text-5` for text and `--accent-1` to `--accent-5` for the clay accent.

After editing, press `Ctrl+R` in Discord or toggle the theme off and on.

## Recommended Vencord plugins

For less tracking and a lighter client: **NoTrack**, **ClearURLs**, **ConsoleJanitor**, **BetterSettings**, **NoTypingAnimation**, **SuperReactionTweaks**, **NoProfileThemes**, **NoOnboardingDelay**, **YoutubeAdblock**.

## Credits

- Made by Mihai.
- Colour inspiration: Claude's interface palette.
- Floating-panel layout selectors and Discord colour-variable mapping adapted from [midnight-discord](https://github.com/refact0r/midnight-discord) by refact0r (MIT).

## License

MIT. See [LICENSE](LICENSE).
