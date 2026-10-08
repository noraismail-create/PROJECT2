# Project Plan

rough map of what we're building and when. move stuff around if it changes, check things off as they get done

## what the game needs (the big pieces)

```
Main Menu
  -> Language Select (python / javascript / ...)
    -> Mini Fight 1 -> catch it
    -> Mini Fight 2 -> catch it
    -> Mini Fight 3 -> catch it
      -> Boss Fight (using the pokemon you caught)
        -> Win screen / Lose screen
```

inside every fight:
1. pick an attack (easy / medium / hard)
2. a code question pops up
3. right answer = damage (more for harder, + type bonus), wrong = no damage
4. enemy attacks back
5. when the enemy is low, try to catch it

## scenes
| scene | what's in it | who |
|---|---|---|
| MainMenu | title, start button, language pick | Systems / UI |
| Battle | both pokemon, hp bars, attack buttons, code question box | Gameplay + Systems / UI |
| Win / Lose | end screens, play again | Systems / UI |
| backgrounds | battle backgrounds for each fight | Art |

## scripts we'll probably need
these are just ideas for names, change them however

| script | does what | who |
|---|---|---|
| BattleManager | runs the turns in a fight | Gameplay |
| Pokemon | hp, type, level, sprite | Gameplay |
| TypeChart | fire/water/grass bonuses | Gameplay |
| ChallengeLoader | reads the questions from challenges.json | Gameplay |
| CodeQuestionUI | shows the question, checks the answer | Systems / UI |
| HealthBar | hp bar on screen | Systems / UI |
| GameManager | remembers language + caught pokemon between scenes | Systems / UI |
| MenuButtons | start, pause, quit, play again | Systems / UI |

## week by week

### weeks 1-2: setup
- [x] make the repo
- [x] add .gitignore
- [x] pick unity version (6.3 LTS)
- [ ] everyone installs unity 6.3 LTS
- [ ] gameplay: make the unity project and push it (see unity-setup.md)
- [ ] everyone clones it and opens it
- [ ] fill in the design doc together
- [ ] art: pick the art style

### weeks 2-3: first playable thing
- [ ] gameplay: battle scene with 2 pokemon and hp going down
- [ ] gameplay: one code question that does damage if right
- [ ] systems/ui: start screen that goes to the battle
- [ ] systems/ui: hp bars
- [ ] art: placeholder sprites + a background
- [ ] everyone: add questions to challenges.json

### midway checkpoint
- [ ] one full fight you can play start to finish
- [ ] start screen + hp display working
- [ ] one level/background ready

### weeks 4-5: the whole game
- [ ] 3 mini fights + boss fight
- [ ] catching
- [ ] type bonuses
- [ ] language select actually changes the questions
- [ ] win / lose screens
- [ ] pause screen
- [ ] music + sound effects
- [ ] final art

### final weeks: polish + build
- [ ] balance damage / difficulty
- [ ] fix bugs
- [ ] export a build and test it on other computers
- [ ] demo!

## still need to decide
- what languages?
- how catching works
- how type bonus + difficulty damage combine
- one try or multiple tries per question
