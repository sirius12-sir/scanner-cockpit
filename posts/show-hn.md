Show HN: Scanner-Cockpit – a single-file, local-first cockpit for running many domains

I run several unrelated domains at once — woodworking, metal, electronics, plus a day job — and the thing that gets you isn't talent, it's the switching cost: every time you return to a domain you have to reload "where was I?".

So I built the opposite of a todo app. It's organized around the *thread* — "what was I last doing here" — not the open items. Each domain is a separate panel; the resume note is the hero, the checklist is secondary. Re-entry cost goes to roughly zero.

It's deliberately the minimal end of local-first: no backend, no account, no sync, no framework. One HTML file. Your data is a plain JSON file on your own disk via the File System Access API (localStorage as fallback). It'll still open in ten years without a toolchain.

What it does NOT do is half the point: no cloud sync, no gamification, no AI. It shouldn't want anything from you.

Live demo: [LIVE-DEMO]
Code: [REPO]

I'm honestly less interested in users than in finding the rare person who operates this way — depth across many unrelated domains, held together by infrastructure rather than willpower. If that's you, I'd like to talk.
