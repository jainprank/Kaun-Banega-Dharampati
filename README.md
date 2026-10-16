# Kaun Banega Dharampati — Punya Ladder

A KBC-style quiz on Jain philosophy. Climb the **Punya Ladder** from 10 to 10,000 Punya across 10 questions, with two Padav (milestones) at Question 5 and Question 10. Each game deals 10 questions at random from the question bank.

## Play
Open `index.html` in a browser, or host the folder with GitHub Pages. No build step; the only external dependency is Google Fonts.

1. Tap **How to Play →** (how-to-play music loops), then **Start Quiz →**
2. 30-second timer on every question. **+30 sec** (top left) adds 30 seconds, once per question. Lifelines **50:50** and **Audience Poll** (run live by the host) are each once per game
3. Clear Question 5 to secure **Padav 1** (250 Punya). A wrong answer after that keeps it, and you may quit at any later question to take it home
4. Answer all 10 correctly to become **Punya Vijeta**
5. A wrong answer or timeout ends the game; **Restart** returns to the rules page

## Layout
```
index.html          # the whole game (HTML + CSS + JS)
audio/              # intro, how-to-play, correct, wrong (ding), tick
images/title.jpg    # title card
images/set1..set5/  # q{1-10}_{idle,correct,wrong}.jpg frames per set
```

The question bank is the `SETS` object near the top of the script in `index.html`: each set lists the correct answer for its 10 questions, and every set joins one pool. To add questions, add a set entry there and its image folder under `images/`.

## Host with GitHub Pages
Repo **Settings → Pages → Deploy from branch → `main` / root**.
