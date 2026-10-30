# Mona’s Octoverse Arcade

**GitHub Day of Learning — 2 Hour Workshop Game Challenge · Canvas Extension Edition**

This repository holds the attendee guide for the workshop. It has two parts:

- **[Open the live attendee website](https://ghlearn.github.io/monas-octoverse-arcade/)**
- **This README**: the full workshop instructions, team rules, agenda, submission steps, judging rubric, and award rules, so you can read everything right here on GitHub.
- **An [Astro](https://astro.build) website** that presents the same guide as a responsive, accessible dark-theme page for attendees.

The site is only an attendee guide. It is not the game. Participants build the game themselves during the workshop.

**Workshop links:** [Instructions](https://gh.io/dol-instructions) · [Discussion and submissions](https://gh.io/dol-discussion). The site's **Workshop links** section includes both clickable links and their supplied QR codes.

The [challenge README](https://github.com/ghlearn/day-of-learning-challenge/blob/main/README.md) is the source of truth for the shared prompt and challenge rules. This attendee guide and the Discussion follow the same guidance.

> **Note:** This is an independent workshop resource. It is **not** an official GitHub event website and is not endorsed by GitHub. GitHub, GitHub Copilot, and the Octocat are trademarks of GitHub, Inc. Supplied GitHub artwork is displayed unaltered. Public-facing mascot use requires approval from GitHub's Brand & Marketing Design team under the [mascot guidelines](https://brand.github.com/graphic-elements/mascots).

---

## Prerequisites, login, and add project to the Copilot app

1. **Install the GitHub Copilot app.** Download and install it from [github.com/features/copilot](https://github.com/features/copilot).
2. **Log in with your provided lab account.** Open the GitHub Copilot app and sign in using the **GitHub Hands-on Labs** account provided to you, rather than your personal GitHub account. The lab environment already has a repository set up for your team, ready to add as a Project. Use that repository rather than creating another one.

> [!NOTE]
> All team members should be able to log in with the one account provided to work on the repository, or you can have one teammate make the changes.

3. **Add your team's repository as a Project in the GitHub Copilot app.** In the app's sidebar, open **Projects** and create a new **Project** named for your team. Select the repository already set up in your GitHub Hands-on Labs environment, not the original `ghlearn/day-of-learning-challenge` template or this attendee-guide repository. Wait for the Project to report that it is ready.

   In the **Project** chat, ask Copilot to start a coding session in your team's repository and open the **Mona's Octoverse Arcade starter** canvas. Confirm its welcome screen appears and its button responds before building. The project-scoped extension is already included; no separate starter download is needed.

Commit and push your team's extension changes so the submitted repository contains the version shown in your demo.

## 🏆 The challenge

Teams build a browser game starring **Mona** the Octocat as the hero and **Copilot** as the sidekick. There is one key requirement: **the game must ship as a Copilot App canvas extension** that can be installed and launched inside the Copilot App itself. Every team starts from one prompt. What you build from it is up to you. After the workshop, judges review every submission and crown the winners.

### Start here: the prompt

Every team starts with this prompt in the Copilot App. It sets the baseline, not the limit.

> In the Mona's Octoverse Arcade starter canvas already included in your team's challenge repository, build the game described here. Keep the existing extension registration in extension.mjs; implement the game in game.html with HTML, CSS, and vanilla JavaScript, with no external build step. Make a game where Mona the Octocat collects green commit-squares while dodging red bugs. Track the score, increase speed over time, and show a game-over screen with a restart button. Copilot appears as a sidekick that gives an encouraging tip every 10 points. Make sure the canvas still opens and the game is playable.

**The baseline:** Mona collects green commit squares and dodges red bugs. The score is tracked, and the speed increases over time. A game-over screen has a restart button. Copilot cheers you on with a tip every 10 points.

**Make it yours:** build what the prompt asks, then take the game somewhere only your team would:

- **Rethink the world**: levels, settings, and a story that make Mona's arcade feel like yours.
- **Invent power-ups**: shields, magnets, merge combos, or boss bugs. Surprise the judges.
- **Give Copilot personality**: make the sidekick funny, helpful, or full of surprises.
- **Find your style**: art direction, animation, and sound that make people want to keep playing.

## 👥 Teams

Up to 150 people may take part. Plan attendance in multiples of 6 so everyone can join a complete team.

- **Exactly 6 people per team**: no smaller or larger teams.
- **Choose a team name** during kickoff. You'll use it on your submission.
- **One shared repository**: keep your team's extension in one repository that judges can open.

With 150 participants, form 25 teams of 6, for 25 team submissions. If your group has fewer than 6 people, join another group. If it has more than 6, split into teams of exactly 6.

## ✅ Core requirement: ship it as a canvas extension

The game can't be a loose HTML file. It must be a **Copilot canvas extension** that:

1. Lives in its own folder, with an `extension.mjs` that **registers a canvas** (the game UI).
2. Can be **installed** into the Copilot App, either with `install_extension` from a GitHub gist or repo folder, or by dropping the folder into the extensions directory.
3. **Runs** when the agent opens it with `open_canvas`. The game renders in the side panel and is playable.

Start from the **working canvas starter already included in your team's lab repository** at `.github/extensions/monas-octoverse-arcade-starter/`. Open that repository as a Copilot App Project and start a coding session there. The project-scoped extension is discovered from the repository. Ask Copilot to open the **Mona's Octoverse Arcade starter** canvas and confirm its welcome-screen button responds. Then build the game in `game.html`; keep the canvas registration in `extension.mjs`. The starter contains no gameplay, so the baseline game and creative choices are the team's work. Use HTML, CSS, and vanilla JavaScript inside the canvas. Keep the game self-contained: no package manifest, dependencies, external assets, or external build step.

**Loading is the setup step:** opening your team's repository as a Project loads the included project-scoped extension. You do not need a separate starter download or to reinstall it for the demo. The installation options above are for trying the extension in another environment.

**Why this raises the bar (in a good way):** participants start with working canvas registration and serving, then build the game itself. They learn how the extension runs in the Copilot App without losing workshop time to setup friction. This is the "GitHub twist" that makes the challenge platform-native.

## ⏱️ Suggested workshop structure (2 hours)

All times below are elapsed from the start of the workshop, not times of day. Install the app and log in before kickoff.

| Time | Phase |
| --- | --- |
| **0:00–0:15** | Kickoff & teams: see the target canvas extension, get the starter prompt and rubric, form teams of exactly 6, and choose a team name |
| **0:15–0:25** | Add the pre-provisioned lab repository as a Copilot App Project, open the **included starter canvas**, and confirm its button responds |
| **0:25–1:15** | Start from the prompt, then build your team's version inside the canvas with the Copilot App |
| **1:15–1:35** | Pick a "power-up" stretch goal (leaderboard, sound, animation, theming, or your own idea) |
| **1:35–2:00** | **Record & submit:** record a demo video of up to 90 seconds and post your submission in the challenge Discussion 🏆 |

## 📮 Submitting

Before the end of the **two-hour workshop**, one teammate posts your team's submission as a **single comment** in the [challenge Discussion](https://gh.io/dol-discussion). Do not submit in a separate Discussion in your team's repository. Include:

1. **Team name**: the name your team chose at kickoff.
2. **Description**: a few sentences about your game, your creative spin, and your power-up.
3. **Demo video**: up to **90 seconds**. Show your team's repository open as a Project with the included extension loaded, open the canvas, and play the game. No separate reinstallation is required. Attach the video to your comment or add a link that judges can access.
4. **Repository link**: your team's repository containing the extension folder. Make sure judges can access it and that your changes are pushed.

The repository must contain the version shown in your demo. Keep any lab credentials out of your video and submission. Use the [submission template in the Discussion](https://gh.io/dol-discussion) to include all four items.

## 🥇 Judging and picking a winner

**How judging works:** after the workshop, judges review every submission's demo video and repository against the 25-point rubric. They choose all three award winners and announce them in the challenge Discussion. There is no audience vote.

### Scoring rubric (25 pts total)

| Criteria | Points | What judges look for |
| --- | ---: | --- |
| **It works**: installs & runs as a canvas | 8 | Extension installs, canvas opens, game is actually playable |
| **Fun factor** | 6 | Is it enjoyable? Would you play again? |
| **GitHub theme** | 5 | Creative use of Mona & Copilot as characters |
| **Polish** | 3 | Visuals, animations, sound, game-over/restart flow |
| **Wow / stretch** | 3 | A power-up feature that surprised the judges |

### Award categories

The **judges decide** all three categories. Each category winner takes home **swag** 🎁.

| 🏆 Award | Recognizes |
| --- | --- |
| **🥇 Overall Winner** | Best total rubric score across all criteria |
| **🎨 Best Design** | The best-looking, most visually striking game (Polish) |
| **🎉 Most Fun** | The game the judges most wanted to keep playing (Fun factor) |

> A team can win more than one category. However, if the Overall Winner also tops another category, that second award rolls to the runner-up to spread the recognition.

## 🎯 Design principles

- ✅ Ship the **rubric up front** so teams build toward what's judged.
- ✅ Provide a **known-good canvas starter** so "install & run" is achievable for everyone.
- ✅ **Reward working software**: the rubric weights "it runs" highest (8 of 25 points).
- ✅ Shared theme, personal spin: every team starts from the same prompt and builds Mona's Arcade, then makes it its own.

## 💡 Ideas for your next canvas extension

Inspiration for after the workshop — not submissions for this competition. Every team builds Mona's Arcade for this challenge, with the shared gameplay requirements and 25-point rubric.

| Idea | Concept | GitHub Twist |
| --- | --- | --- |
| **"Ask Mona" Chatbot** | A rule-based/scripted Q&A assistant UI | Mona answers Git/GitHub beginner questions; Copilot suggests follow-ups |
| **Commit Streak Tracker** | A habit/streak tracker | Themed as a "contribution graph": earn Mona badges for streaks |
| **Octo-Quiz** | Timed trivia game | Git/GitHub trivia; Copilot gives hints, Mona celebrates wins |
| **PR Review Simulator** | Card-swipe game (approve/request changes) | Learn code-review etiquette; Mona is the author, Copilot the reviewer |
| **Mona's Sticker Maker** | Canvas drawing + Octocat generator | Compose your own Octocat; export as PNG |

## Learn by doing with GitHub Skills

GitHub Skills offers free, hands-on courses you complete in public GitHub repositories. Follow step-by-step guidance and get automated feedback as you learn.

Keep learning at [gh.io/gh-skills](https://gh.io/gh-skills). The site's **Learn by doing with GitHub Skills** section follows the future canvas ideas and includes this link and its supplied QR code.

---

## 🖥️ Running the attendee website

This section is for website maintainers, not for building the challenge game. Attendees use the included canvas starter; they do not need Node.js, npm, or a website build step for the game.

### Prerequisites

- [Node.js](https://nodejs.org/) **22.12.0 or later** (required by Astro 7)
- npm (included with Node.js)

### Commands

Run these from the repository root:

| Command | Action |
| --- | --- |
| `npm install` | Install dependencies |
| `npm run dev` | Start the local dev server at `http://localhost:4321` |
| `npm run build` | Build the static production site to `./dist/` |
| `npm run preview` | Preview the production build locally |

### Build output

`npm run build` writes a fully static site to `dist/` (an `index.html` plus the assets in `public/`). You can deploy that folder to any static host.

`astro.config.mjs` reads two optional environment variables: `SITE_URL` (the site origin) and `BASE_PATH` (the sub-path). Locally they're unset, so the site is served from `/`. To test a sub-path build:

```bash
SITE_URL=https://arilivigni.github.io BASE_PATH=/monas-octoverse-arcade npm run build
```

### Deploying to GitHub Pages

`.github/workflows/deploy-pages.yml` builds the site and publishes it to GitHub Pages. It runs on every push to `main` and can also be started by hand from the **Actions** tab (**Run workflow**). The workflow gets the correct origin and sub-path from `actions/configure-pages`, so links and assets work at `https://<owner>.github.io/<repo>/` or on a custom domain.

Keep this as the only Pages deployment workflow. A second workflow can overwrite the site with a build missing `SITE_URL` and `BASE_PATH`, causing styles, images, and the favicon to return 404 errors on repository URLs.

One-time setup:

1. Go to **Settings → Pages** in the repository.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. Push to `main` (or run the workflow). The site URL appears in the workflow run summary and in **Settings → Pages**.

> **Private repository note:** GitHub Pages for private repositories requires a GitHub Pro, Team, Enterprise Cloud, or Enterprise Server plan. On GitHub Free, make the repository public to publish the site. On Enterprise Cloud you can also limit who can view the site.

The page loads no remote images, fonts, or scripts at runtime. The only JavaScript on the page is a small inline script that turns on the "Copy prompt" button, and the page works without it.

### Project structure

```text
.
├── .github/workflows/
│   └── deploy-pages.yml      # Build and deploy to GitHub Pages
├── astro.config.mjs          # Astro configuration (static output, SITE_URL/BASE_PATH support)
├── docs/
│   └── speaker-demo-runbook.md # Speaker-only demo runbook (not published on the site)
├── package.json              # Scripts and the single dependency: astro
├── public/
│   ├── favicon.svg           # Neutral arcade icon, not a mascot or GitHub logo
│   └── images/
│       ├── dol-instructions.png # Supplied instructions QR code
│       ├── dol-discussion.png   # Supplied Discussion QR code
│       ├── gh-skills.png        # Supplied GitHub Skills QR code
│       ├── arcade-hero.png   # Supplied Mona and green-block landscape
│       └── hero-arcade.svg   # Previous artwork, no longer displayed
└── src/
    ├── layouts/
    │   └── Base.astro        # HTML shell, metadata, favicon, skip link
    ├── pages/
    │   └── index.astro       # The attendee guide page (all workshop content)
    └── styles/
        └── global.css        # Dark event theme, responsive layout, focus and reduced-motion styles
```

### Design and accessibility notes

- Neutral ink and charcoal surfaces, GitHub green (`#0FBF3E`) as the primary accent, and restrained Copilot purple, following the [GitHub Brand Toolkit](https://brand.github.com/foundations/color). Bright secondary colors stay primarily in the supplied artwork.
- The main Mona landscape and all three supplied QR codes (Instructions, Discussion, and GitHub Skills) are displayed without recoloring, cropping, or overlaid text. The final "One Mona. Endless possibilities." section is text-only, with no artwork gallery.
- Mascots illustrate the creative challenge, rather than serving as the site's logo or explaining instructions. Public-facing mascot use still requires GitHub Brand approval.
- The page uses semantic HTML landmarks, headings, tables, and lists, plus a skip link.
- The navigation is keyboard-accessible, and focus states are visible.
- Layouts are responsive down to 320px wide.
- `prefers-reduced-motion` turns off page animation.
- Text and accent colors meet WCAG AA contrast against their backgrounds.
