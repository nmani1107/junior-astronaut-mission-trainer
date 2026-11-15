# Junior Astronaut Mission Trainer

**NASA Space Apps Challenge 2026 — "Build a Junior Astronaut Mission Trainer"**

Play it live (no download, no account): https://nmani1107.github.io/junior-astronaut-mission-trainer/

A fun, interactive game for children ages 7–12 that teaches what it really takes to train and prepare for a Moon or Mars mission — living in space, doing science, staying healthy, and working as a team — using real NASA data.

## How to play

1. Open the link above on any phone, tablet, or laptop (2016–2026 browsers).
2. Tap **Start with Voice Guide** (or **Play without voice**), type your first name — it stays on your device only, just for your training badge.
3. Pick your level: **Easy** (ages 7–8, more time, fewer hazards) or **Commander Hard** (age 10+, less time, more hazards).
4. Play the 6 training missions. Each win finishes one training day. Finish all 7 days and all 4 main missions to become a **Commander** and earn your certificate.
5. Switch cadets any time — each cadet keeps their own progress on the same device. No login, no account, nothing is sent anywhere.

## The 6 missions

| Mission | What you do | What it teaches |
|---|---|---|
| Spacewalk Training | Catch falling tools and supplies, dodge falling asteroids and rocks | Working outside a spacecraft, staying safe in space |
| Exercise in Space | Tap the glowing pad as fast as you can — the astronaut does the exercise on screen | Why astronauts exercise every day in microgravity (OSDR health data) |
| Moon Base Keeper | Balance oxygen, food, power, and your radiation shield to keep the base alive | **The Big Trade-Off:** oxygen, power, and food compete on one power supply — every choice has a real cost |
| Space Weather Watch | Watch a NASA motion (a rocket launching, a solar flare, a CME, auroras…) and answer "What is this called?" | Live space weather from NASA DONKI, radiation risk, and shielding (RadLab) |
| Moon Base Defender (bonus) | Clear friendly Moon Dust, answer NASA questions to get stronger and bring light to the base | Teamwork, light, and cleaning up a base |
| Earth to Moon Journey (bonus, story) | Steer to the Moon, dodge asteroids, fix a mid-flight problem with 3 questions, meet Moon Friends, fly home | Communication delay (Mission Control messages arrive late), asteroids, and the journey home with a 5-4-3-2-1 countdown |

**Mars side:** pick a real Mars Trek landing site — Jezero, Gale, or Elysium — with its real conditions, and see the live Mars rover photo on the way.

**Communication delay:** in the Journey, messages from Mission Control visibly travel and arrive after 1.3 seconds, and the game explains the real Mars delay of about 22 minutes.

**Replayability:** Weather Watch shuffles its motions and answers every game on top of live DONKI data, Moon Base events stay random, and Spacewalk drops vary — no two playthroughs are the same.

## How we meet the challenge

See the **"🏆 How We Meet the Challenge"** tab in the game's Dashboard — it lists all 9 official requirements and exactly what we built for each one, in plain words.

In short: a working prototype for ages 7–12, a lunar/Martian outpost with real decisions, a clear trade-off mechanic, life support / radiation shielding / power budgeting / food production / communication delay, real NASA data shaping the play, browser-playable with no download or account, and plain language with jargon (radiation dose, microgravity, sol) explained in context.

## NASA data & sources used — and why

| Source | Live or curated | Why we used it |
|---|---|---|
| NASA Open APIs (APOD + Mars Rover Photos) | **LIVE** | Real space pictures in "Live from NASA" — a real Mars photo and today's Astronomy Picture of the Day |
| DONKI space weather database | **LIVE** | Real solar flares, CMEs, and geomagnetic storms drive Space Weather Watch |
| NASA Open Science Data Repository (OSDR) | Curated real facts | Real astronaut health findings shape Exercise — how space affects the human body |
| RadLab (NASA Radiation Laboratory) | Curated real facts | Real radiation risk and shielding facts shape Moon Base Keeper and Space Weather Watch |
| Mars Trek | Curated real facts | Real Mars landing sites and conditions shape the Mars choice in the Journey |
| CSA — Astronaut Training: Get Ready For Space | Curated | How astronauts really train — physical training, simulations, mission prep |
| CSA — Your Body in Space | Curated | How the body adapts to microgravity, exercise, and health in space |

Curated data is labelled **"Curated facts — not live"** in the game; live data is labelled **LIVE**. Nothing static is presented as live. All sources are also listed and linked inside the game, in the Dashboard's **NASA Data & Sources Used** tab.

## Voices, music, and accessibility

- **Family voices:** the Welcome and each mission's instructions are spoken by our own family — recorded by us, in the game. (The Welcome voice is Mani's; Spacewalk and Journey are our son's; Exercise and Defender are our daughter's; Moon Base Keeper and Weather Watch are Gracy's.)
- **Browser voice fallback:** if a recording can't play, the browser's own voice reads the same words instead.
- **Word-by-word highlighting** with auto-scroll on every spoken line, so young readers can follow along.
- **Background music:** a soft original music-box tune, only inside missions, that ducks to a whisper whenever a voice speaks. Sound and music can be switched off from the first page.
- **Science pop-ups:** every mission has a 🔬 "The Science Behind This" button — science only, with audio that plays by itself, Stop, and Listen again.
- **Difficulty:** Easy (ages 7–8) and Commander Hard (age 10+), saved in your profile.

## Tech

- One single self-contained `index.html` — plain HTML, CSS, and JavaScript. No framework, no build step, no backend, no server, no database.
- Progress is saved in the browser's localStorage on that device only. Nothing is sent anywhere.
- Works on phones, tablets, and laptops (2016–2026 browsers). Voice/audio may fall back to text-only on very old browsers.

## Team

- **Manikandan (dad, "Mani")** — builder, Welcome voice
- **Gracy (mom)** — Moon Base Keeper + Weather Watch voices
- **Thanesh (son, age 10)** — Spacewalk + Journey voices, game designer and lead playtester
- **Mounaashree (daughter, age 8)** — Exercise + Defender voices
- We are a family team: dad and mom are helping our kids Thanesh (10) and Mounaashree (8) complete this project.
- Built with help from **Muse (Remo)**, our AI assistant — AI tools used are disclosed here, as the challenge requires. No NASA branding or logos are used.

## How we built it — the kids tested it, then made it better

The kids didn't just play the game — they tested it and then told us what to change, and we built their ideas in:

1. **Thanesh (10) played Spacewalk and said it was too easy and simple.** After testing, he suggested: instead of walking around collecting tools, make tools and asteroids fall from the top — dodge the rocks, catch the tools, collect enough to move to the next level. We rebuilt Spacewalk that way.
2. **Thanesh played Exercise and said the screen needed motion.** After testing, he suggested: show the astronaut actually doing the exercise — running when the pad says running. We added matching motion animations for every exercise.
3. **Thanesh played Space Weather Watch and said reading a passage first was boring.** After testing, he suggested: show a NASA motion instead (like a rocket taking off) and ask "What is this called?" We rebuilt it as a 7-question motion quiz.
4. **Thanesh played the Journey and said it needed more excitement.** After testing, he suggested: asteroids coming down to dodge, a hit just puts you back (respawn, not game over), a proud "Well done!" voice when you reach the Moon, a 5-4-3-2-1 take-off countdown for the flight home, about 15 seconds from Earth to the problem and 20 seconds from there to the Moon, and lots of description, stars, and planets everywhere. We built all of it.
5. **Thanesh also said Moon Base Keeper and Moon Base Defender were already good** — leave those two alone. We did.
6. **Mounaashree (8) playtested every mission** on Easy level and recorded the Exercise and Defender voices.

## Playtesting

Played and tested by our own children — Thanesh (10) and Mounaashree (8) — throughout the hackathon, and shared with friends and family to playtest, as the challenge recommends. Their testing directly shaped the game: the falling Spacewalk, the Exercise motion, the Weather Watch motion quiz, and the Journey asteroids all came from Thanesh's suggestions after he played each mission.

## Submission

- **Final project (playable):** https://nmani1107.github.io/junior-astronaut-mission-trainer/
- **Source code:** this repo (`index.html`)
- **Demo:** 30-second video (kids playing) or 7-slide deck — see the team's Project page on spaceappschallenge.org
- Submitted by the team themselves before Sunday, November 15, 2026, 11:59 PM local time.
