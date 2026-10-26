<div align="center">

# Hot Jungle

**Hot Jungle («Огненные джунгли») is a run-and-gun arcade game in a single HTML page: five missions through the jungle, each ending with a boss. It runs in the browser with no server and no internet: open `index.html` or play it online.**

[**▶ Play online →**](https://alexalesha.github.io/HotJungle/) &nbsp;·&nbsp; [Русская версия этого файла](README.ru.md)

[![Status](https://img.shields.io/badge/status-stable-brightgreen)](#) [![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE) [![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML) [![Website](https://img.shields.io/badge/Website-open-0A84FF?logo=googlechrome&logoColor=white)](https://alexalesha.github.io/HotJungle/) [![Built with Claude Code](https://img.shields.io/badge/Built_with-Claude_Code-D97757?logo=claude&logoColor=white)](https://claude.com/claude-code)

Code, tests and docs are written by Claude (Anthropic) in Claude Code. Ideas, testing and decisions - Alexey.

</div>

> Fan-made game, not affiliated with any rights holder. Pixel sprites and the font are drawn by code.

The interface is in Russian.

![Menu](docs/screens/menu.png)

![River at sunset](docs/screens/play.png)

![Walker boss](docs/screens/boss.png)

## What is in the game

- **Campaign of five missions:** a jungle fort, a river at sunset, caves, a secret base and the tower assault; two checkpoint flags per mission.
- Power-ups drop from enemies and flying capsules: spread shot, rapid fire, a piercing laser and a one-hit shield; a weapon is lost with a life.
- Snipers show a red aiming beam first, mines beep, the walker sends a shock wave along the ground - jump over it.
- Mission select, achievements and records, settings, gamepad support; its own pixel font; music and sounds are synthesised with WebAudio.

## Controls

| Key | Action |
|---|---|
| A / D or arrows | run |
| W | aim up (diagonally while running) |
| S | lie down; S + jump drops through a platform |
| Space | jump |
| J / X or left mouse button | fire (hold for bursts) |
| Esc | pause |

Keys can be changed in the settings where the game offers it; a gamepad works too where noted above.

## Run locally

Open `index.html` in Chrome, Edge or Firefox. Everything is in the repository; nothing is downloaded.

## Tests

The laws are Playwright tests in `tests/`. They open the page by its file address in headless
Chromium, one at a time:

```
npm install
npx playwright install chromium
npm test
```

Mouse capture in the tests is always a stub (a real `requestPointerLock` in headless Chromium on
Windows can clip the user's cursor).
The pictures above were made headless by the screenshot script of the Hub collection.

## History

The game was made in the [Hub](https://github.com/ALEXalesha/ALEXalesha.github.io) collection, where it also runs in the Hub ([play there](https://alexalesha.github.io/)). This repository carries the game with its commit history.

## Licence

MIT, see [LICENSE](LICENSE).
