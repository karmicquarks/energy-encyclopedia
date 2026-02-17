# Karmic Quarks Connect – Renewables Encyclopedia

A client-side, single-file interactive encyclopedia/social media placform to primarily discuss renewable & new energy technologies.

Built with pure HTML, CSS, and JavaScript — **no backend**, no frameworks, no build step.

Live demo:  
https://valeman0420.github.io/energy-encyclopedia/  
(or replace with your actual GitHub Pages URL once deployed)

## Features

- **User accounts** — Visitor / Basic / Moderator / Admin roles (demo credentials included)
- **Registration & login** with email + password (stored in localStorage – demo only)
- **Section-level content** for 8 renewable energy types (Wind, Solar, Hydro, Thermal, Biomass, Geothermal, Tidal, Wave)
- **Admin/Moderator tools**:
  - Edit section text
  - Add/update header image & video (via URL – YouTube or direct .mp4)
- **Comment system**:
  - Threaded replies with collapse/expand
  - Edit & delete own comments
  - Moderators/admins can delete/edit any comment
  - Emoji reactions (👍 ❤️ 😂 etc.) with picker
  - @mentions with auto-suggest dropdown
- **Notifications**:
  - Reply & mention alerts (toast + bell icon)
  - Cross-tab sync via `storage` event
- **Accessibility & input**:
  - Speech-to-text dictation (voice → text)
  - Text-to-speech read-aloud with pause/resume
- **Rich comments**:
  - Markdown-style auto-linking & image embedding
  - Voice replies (short recordings – limited by localStorage)
- **Fully offline-capable** after first load (data in localStorage)

## Technologies

- HTML5
- CSS3 (vanilla)
- Vanilla JavaScript (ES6+)
- Web APIs:
  - Web Speech (SpeechSynthesis & SpeechRecognition)
  - MediaRecorder (voice replies)
  - localStorage + `storage` event
  - Notification toasts

## How to Run Locally

1. Clone or download this repo
2. Open `index.html` directly in a modern browser (Chrome/Edge recommended)
   - `file://` protocol works fine — no server needed

## How to Deploy (GitHub Pages)

1. Create a repository (e.g. `energy-encyclopedia`)
2. Upload or paste the content into `index.html`
3. Go to **Settings → Pages**
4. Set source → Branch: `main` / Root
5. Wait 1–2 minutes → your site is live at  
   `https://<your-username>.github.io/<repo-name>/`

## Demo Accounts

| Role       | Email                  | Password | Notes                     |
|------------|------------------------|----------|---------------------------|
| Admin      | admin@example.com      | admin    | Full edit/delete powers   |
| Moderator  | mod@example.com        | mod      | Can moderate comments     |
| Basic User | user@example.com       | user     | Can comment & react       |

(You can register new basic users too)

## Limitations & Notes

- All data is stored in browser `localStorage` → **not shared between devices/browsers**
- No real-time multi-user chat (client-side only)
- Voice replies & media are limited by ~5–10 MB storage quota
- No server-side persistence or authentication (demo / educational project)

## Contributing

Pull requests welcome!

Especially appreciated:

- Better markdown parser for comments
- Dark mode toggle
- More emoji sets / reaction sorting
- Accessibility improvements (ARIA labels, keyboard nav)
- Refactoring repetitive section HTML into JS template

## License

MIT License – feel free to fork, modify, and use commercially.

Made with ❤️ in Austin, Texas  
© 2026 V 420 (@valeman0420)
