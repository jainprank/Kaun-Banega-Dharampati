# Kaun Banega Dharampati — Punya Ladder

A KBC-style quiz on Jain philosophy. Climb the **Punya Ladder** from 10 to 10,000 Punya across 10 questions, with two Padav (milestones) at Question 5 and Question 10.

## Play
Open `index.html` in a browser, or host the folder with GitHub Pages. No build step; the only external dependency is Google Fonts.

1. Tap **How to Play →** (how-to-play music loops), then **Start Quiz →**
2. Choose a set: Set 1 (Q1–Q10), Set 2 (Q12–Q21), Set 3 (Q22–Q31), Set 4 (Q32–Q41), Set 5 (Q42–Q50)
3. 30-second timer on every question; lifelines **50:50** and **Audience Poll** (run live by the host), once each per game
4. Clear Question 5 to secure **Padav 1** (250 Punya). A wrong answer after that keeps it, and you may quit at any later question to take it home
5. Answer all 10 correctly to become **Punya Vijeta**

## Layout
```
index.html          # the whole game (HTML + CSS + JS)
audio/              # intro, how-to-play, correct, wrong (ding), tick
images/title.jpg    # title card
images/set1..set5/  # q{1-10}_{idle,correct,wrong}.jpg frames per set
```

Correct answers live in the `SETS` object near the top of the script in `index.html`.

## Host with GitHub Pages
Repo **Settings → Pages → Deploy from branch → `main` / root**.
