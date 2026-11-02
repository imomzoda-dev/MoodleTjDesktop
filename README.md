<p align="center">
  <img src="resources/icon.png" width="112" alt="Moodle.tj Desktop" />
</p>

<h1 align="center">Moodle.tj Desktop</h1>

<p align="center">
  The official <b>Windows</b> and <b>macOS</b> app of the <a href="https://moodle.tj">Moodle.tj</a> learning platform —
  courses, lessons, quizzes, coding tasks, an AI tutor, the digital library, a teacher cabinet and analytics. Fast, and even offline.
</p>

<p align="center">
  <a href="https://github.com/imomzoda-dev/MoodleTjDesktop/releases/latest"><img alt="Latest version" src="https://img.shields.io/github/v/release/imomzoda-dev/MoodleTjDesktop?label=version&color=c0532f" /></a>
  <img alt="Windows 10/11" src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?logo=windows&logoColor=white" />
  <img alt="macOS 12+ Apple Silicon" src="https://img.shields.io/badge/macOS-12%2B%20·%20Apple%20Silicon-111111?logo=apple&logoColor=white" />
  <a href="https://github.com/imomzoda-dev/MoodleTjDesktop/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/imomzoda-dev/MoodleTjDesktop/total?color=2ea043" /></a>
</p>

<p align="center">
  <a href="https://github.com/imomzoda-dev/MoodleTjDesktop/releases/latest"><b>⬇ Download for Windows</b></a> — <code>Moodle.tj-Desktop-Setup-&lt;version&gt;.exe</code>
  <br />
  <a href="https://github.com/imomzoda-dev/MoodleTjDesktop/releases/latest"><b>⬇ Download for macOS</b></a> — <code>Moodle.tj-Desktop-&lt;version&gt;-arm64.dmg</code>
  <br /><br />
  <a href="README.ru.md">Русский</a> &nbsp;·&nbsp; <a href="CHANGELOG.md">What's new</a>
</p>

> [!IMPORTANT]
> **macOS: run one command before the first start.** After dragging the app into *Applications*, open **Terminal** and run:
>
> ```bash
> xattr -dr com.apple.quarantine "/Applications/Moodle.tj Desktop.app"
> ```
>
> Without it macOS refuses to open the app (*“cannot be opened”* or *“is damaged”*), because it is not signed with an Apple Developer ID. Once per installation is enough — [details](#macos-apple-silicon-m1m5).

<p align="center">
  <img src="docs/screenshots/06-home-light.png" width="49%" alt="Home, light theme" />
  <img src="docs/screenshots/07-home-dark.png" width="49%" alt="Home, dark theme" />
</p>

## One app, two systems

The same app, the same account and the same features on Windows and on a Mac — each with the habits of its system.

<p align="center">
  <img src="docs/screenshots/flow-workspace.png" width="49%" alt="Workspace on Windows" />
  <img src="docs/screenshots/mac-workspace.png" width="49%" alt="Workspace on macOS" />
  <br /><sub>The Workspace on Windows (left) and on macOS (right).</sub>
</p>

| | Windows | macOS |
|---|---|---|
| Processors | x64 | Apple Silicon (M1–M5) |
| Install | `Setup-<version>.exe`, with an *Update 1.x → 1.y* page | `.dmg`, drag to *Applications* |
| Updates | inside the app, SHA-512 checked, differential download | inside the app, SHA-512 and signature checked, the app replaces itself |
| Updates follow | the newest **Windows** build | the newest **Mac** build |
| Sign-in token kept in | Windows DPAPI | macOS Keychain |
| Look | Mica / Acrylic window, native caption buttons | translucent window, traffic lights, ⌘ shortcuts |
| Workspace terminal | PowerShell, CMD, Git Bash | zsh (your login shell), PowerShell if installed |

## What's new in 1.2

- **A new lesson page**: the text in a card with coloured titles and lists, code in dark code cards with line numbers and *Copy*, *In this lesson* and *Course contents* on the right, and a lesson text size setting.
- **Teacher cabinet**: lessons in every course language, *New lesson*, *Duplicate*, drag-and-drop order, the lesson language, quiz results of every student, course analytics with *Remind*.
- **Site analytics in the app** for administrators: overview with trends, students at risk, campaigns with sending and exclusions, the delivery log, student cards, CSV export.
- **macOS version** with in-app updates; Windows and macOS update independently, each from its own builds.
- **Update card on the sign-in screen**, and a sign-in that needs one request instead of two.
- A new **news** page, the **Workspace**, a **visual lesson editor**, a smart cache.

Full list — [CHANGELOG](CHANGELOG.md).

## Features

**Learning**
- Home with a personal greeting, streak and progress, *Continue learning*, today's plan, upcoming deadlines and popular courses.
- *All courses* with a large search, a filter panel (subject, level, language, price) and sorting; enrolment and enrolment requests with a document.
- Lessons in a card, as on the site: titles and contents on the right, the course outline, code cards with line numbers and *Copy*, an adjustable text size; video that resumes where you stopped, PDF materials in a built-in viewer, discussion with replies and likes.
- **AI tutor** in a side panel: live streamed answers, Markdown and highlighted code, model choice, history.
- Quizzes with a timer, single/multiple/text questions, protection against leaving by accident, a detailed review.
- Assignments with drag-and-drop upload, grade and teacher feedback.
- Coding tasks in the Monaco editor: *Run* with input, *Submit* with verdicts (AC/WA/CE/RE/TLE) and per-test results; an online compiler with your own files.

**Workspace** — a code workspace on your computer: a project folder with the file explorer, code search and `Ctrl+P` / `⌘P`, the Monaco editor with tabs, a real terminal, Git (changes, commits, branches, pull/push) and the project's tasks in one click.

**Library** — showcase, collections, authors, search, a PDF/EPUB reader that remembers your page, notes and quotes, *My shelf*, purchase requests for paid books (the site's rules — watermark and daily limit — always apply).

**Community** — news with a top story, *Top news*, *Popular* and tags, likes and comments; course forums; the community chat with pictures, replies and read marks; a notification centre with system notifications and a badge.

**Motivation** — achievements, streaks and an activity calendar, the leaderboard, certificates (claim, view, save, verification link) and certificate verification.

**Teachers** — courses (create, edit, translations, cover, Markdown preview); lessons in every course language with *New lesson*, *Duplicate* (with the quiz and materials), *Open as a student* and drag-and-drop order; a visual lesson editor as on the site; materials; a quiz builder with bulk import and **quiz results of every student**; assignments and grading; coding tasks with tests and a reference-solution check; an AI assistant for lesson authors; **course analytics** — funnel, churn risk, the lesson where students stop, daily activity, every student with *Remind*.

**Administrators** — premium and enrolment requests, messages, announcements, users; **analytics in the app** — overview with trends, students at risk, campaigns (enable, test, send to one, the selected or everyone, exclude), the delivery log, student cards, CSV export; and the full site admin in a secure, auto-signed-in window.

**Desktop quality** — three interface languages (Tajik by default, Russian, English), light/dark themes, `Ctrl+K` / `⌘K` command palette, keyboard shortcuts, offline mode with a queue of actions sent when the connection returns, `moodletj://` links, a tray icon, start at login, automatic updates.

## Screenshots

**Sign-in and updates**

<p align="center">
  <img src="docs/screenshots/01-login-light.png" width="49%" alt="Sign in, light" />
  <img src="docs/screenshots/21-login-update.png" width="49%" alt="An update offered on the sign-in screen" />
</p>

**Learning**

<p align="center">
  <img src="docs/screenshots/27-lesson-light.png" width="49%" alt="Lesson with code cards and contents, light" />
  <img src="docs/screenshots/28-lesson-dark.png" width="49%" alt="Lesson, dark theme" />
</p>
<p align="center">
  <img src="docs/screenshots/18-lesson-tutor-light.png" width="49%" alt="Lesson with the AI tutor" />
  <img src="docs/screenshots/flow-coding-check.png" width="49%" alt="Coding task" />
</p>
<p align="center">
  <img src="docs/screenshots/08-catalog-dark.png" width="49%" alt="All courses" />
  <img src="docs/screenshots/16-news-light.png" width="49%" alt="News" />
</p>
<p align="center">
  <img src="docs/screenshots/10-library-light.png" width="49%" alt="Library" />
  <img src="docs/screenshots/11-achievements-dark.png" width="49%" alt="Achievements" />
</p>

**Teachers**

<p align="center">
  <img src="docs/screenshots/22-teacher-lessons.png" width="49%" alt="Lessons of a course in every language" />
  <img src="docs/screenshots/23-course-analytics.png" width="49%" alt="Course analytics" />
</p>
<p align="center">
  <img src="docs/screenshots/flow-lesson-editor.png" width="49%" alt="Visual lesson editor" />
  <img src="docs/screenshots/flow-attempt-review.png" width="49%" alt="A student's quiz attempt" />
</p>

**Administrators**

<p align="center">
  <img src="docs/screenshots/24-admin-analytics-dark.png" width="49%" alt="Site analytics, dark theme" />
  <img src="docs/screenshots/25-analytics-student.png" width="49%" alt="Student card" />
</p>
<p align="center">
  <img src="docs/screenshots/26-analytics-campaign.png" width="49%" alt="Notification campaign" />
  <img src="docs/screenshots/15-compiler-dark.png" width="49%" alt="Online compiler" />
</p>

## Installation

### Windows

1. Download `Moodle.tj-Desktop-Setup-<version>.exe` from [Releases](https://github.com/imomzoda-dev/MoodleTjDesktop/releases/latest).
2. Run it and choose the folder. Updating keeps your sign-in, settings and offline data.
3. The installer is **not code-signed**: Windows SmartScreen may show *“Windows protected your PC”* — click **More info → Run anyway**.

**Requirements:** Windows 10/11 x64, 4 GB RAM, about 400 MB of disk space, a Moodle.tj account.

### macOS (Apple Silicon: M1–M5)

1. Download `Moodle.tj-Desktop-<version>-arm64.dmg` from [Releases](https://github.com/imomzoda-dev/MoodleTjDesktop/releases/latest), open it and drag **Moodle.tj Desktop** into **Applications**.
2. **Before the first start**, open **Terminal** (*Spotlight* `⌘ Space` → type *Terminal* → `Return`, or *Applications → Utilities → Terminal*) and run:

   ```bash
   xattr -dr com.apple.quarantine "/Applications/Moodle.tj Desktop.app"
   ```

   The command asks for nothing and prints nothing — that means it worked. It removes the *downloaded from the internet* (quarantine) mark that macOS puts on every app without an Apple Developer ID; with that mark macOS says the app *“cannot be opened”* or *“is damaged and can't be opened”*.
3. Open **Moodle.tj Desktop** from *Applications* or *Launchpad*.

> [!NOTE]
> - The command is needed **once per installation** from the DMG (and again if you install a new DMG by hand). Updates made inside the app need nothing: the app removes the mark itself.
> - If the app is in another folder, use its path instead of `/Applications/…`.
> - Without Terminal: try to open the app once, then go to **System Settings → Privacy & Security** and click **Open Anyway**.

**Requirements:** macOS 12 or later on Apple Silicon, a Moodle.tj account.

## Updates

The app checks GitHub Releases at start and every 4 hours (automatic checks can be turned off in *Settings*). A new version appears as a card in the sidebar — and on the sign-in screen, so you can update even before signing in. *Update* downloads the file and checks its SHA-512; *Restart and update* installs it and opens the new version.

- **Windows** reads `latest.yml`, **macOS** reads `latest-mac.yml`: each system takes the newest release that has its own build, so one system never waits for, or fails on, the other's release.
- On a Mac keep the app in **Applications**: it replaces itself there. Started from the DMG or from a folder without write access, *Update* opens the new DMG instead.

## Privacy and security

- Your password is never stored. The server issues a token for this device; it is encrypted by the system (Windows DPAPI or the macOS Keychain) and never reaches the interface, logs or files in plain text.
- *Sign out* ends the session on this device only and removes this account's offline data.
- No telemetry. The app talks to `moodle.tj` (and, for Gemini models of the AI tutor, to Google), and to GitHub to check for updates.
- Strict sandbox: context isolation, no Node.js in the interface, a strict Content-Security-Policy, all server HTML sanitized, no device permissions.

## Versions

| Version | Date | Systems | Downloads |
|---|---|---|---|
| [1.2.3](https://github.com/imomzoda-dev/MoodleTjDesktop/releases/tag/v1.2.3) | 02.11.2026 | Windows, macOS | ![downloads](https://img.shields.io/github/downloads/imomzoda-dev/MoodleTjDesktop/v1.2.3/total) |
| [1.2.2](https://github.com/imomzoda-dev/MoodleTjDesktop/releases/tag/v1.2.2) | 02.11.2026 | Windows, macOS | ![downloads](https://img.shields.io/github/downloads/imomzoda-dev/MoodleTjDesktop/v1.2.2/total) |

Earlier versions — see the [CHANGELOG](CHANGELOG.md).

## License

© 2026 Imomzoda Mehriddin. Free to use — see [LICENSE.txt](LICENSE.txt).
