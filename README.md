# Trivia Master Gulpin 🎮

A fun trivia game with a Pokémon twist! Test your knowledge with questions from the Open Trivia Database, plus some custom questions thrown in for good measure. But watch out get an answer wrong and Gulpin will assign you a punishment!

## What's This?

This is a browser-based trivia game that combines general knowledge questions with fanmade ones. The catch? Every time you get something wrong, you face a random punishment (like dropping all your weapons in a game, doing a speedrun challenge, or speaking Spanish until the next question). And if you hear the word "GULPIN" a lot, that's intentional it might even replace words in your questions!

## Features

- **Mixed Question Sources**: Pulls from the Open Trivia Database API and cycles through custom questions
- **Text-to-Speech**: Questions are read aloud with a fun twist "GULPIN" gets replaced with an actual Gulpin cry
- **Random Punishments**: Wrong answers trigger creative punishments from a pool that gets refilled when exhausted
- **Visual Feedback**: Correct answers turn green, wrong ones turn red
- **Auto-Loading**: New questions load automatically every 7 minutes
- **Gulpin Chaos Mode**: The chance of words being replaced with "GULPIN" increases by 10% each time you get that specific punishment

## How to Play

Just open `index.html` in your browser and you're good to go! No build steps, no dependencies pure vanilla JavaScript.

1. Wait for the question to be read aloud
2. Click one of the four answer buttons
3. If you're right, you're safe... for now
4. If you're wrong, accept your punishment with grace (or not)
5. Next question loads automatically after 7 minutes

## Punishments

Some examples of what you might face:
- Drop all weapons (if you're gaming)
- Complete a shrine in Tears of the Kingdom
- Do a Random Battle in Pokémon Showdown
- Draw a random Pokémon from memory
- Recite Steamed Hams from memory (good luck!)
- The dreaded "Chance of gulpin replacing words increased by 10%"

...and many more!

## Technical Stuff

Built with:
- Vanilla JavaScript (no frameworks!)
- Web Speech API for text-to-speech
- Open Trivia Database API for questions
- Pure CSS for styling

The code uses modern JavaScript features like:
- `const`/`let` instead of `var`
- Arrow functions
- Array methods like `.map()` and `.forEach()`
- Async/await for API calls
- Fisher-Yates shuffle algorithm

## Question Cycle

The game alternates between API questions and fanmade questions:
- First 4 questions: From Open Trivia Database
- Next question: Random fanmade question
- Repeat!

Fanmade questions shuffle when you've been through them all.

## Customizing

Want to add your own questions? Edit `fanmade-questions.js`:

```javascript
["Category", "Your question?", "Correct answer", "Wrong 1", "Wrong 2", "Wrong 3"]
```

Want different punishments? Edit the `punishments` array in `index.html`.

## Credits

Questions powered by [Open Trivia Database](https://opentdb.com/)

Gulpin cry from [Pokémon Showdown](https://play.pokemonshowdown.com/)

## License

Feel free to use this for whatever! It's just a silly trivia game.

---

*Made with ❤️ and way too much time*