# Tamagotchu

Tamagotchu is a browser-based interactive chatbot project about digital communication, personality, and the blurred line between human and machine responses. It wraps a RiveScript conversation engine in a retro Tamagotchi-style interface with scanlines, video states, button-triggered animations, and a score counter.

The bot's replies are assembled from different response styles and sources, including Siri-like answers, chatbot-style answers, ELIZA-inspired prompts, forum-like responses, and intentionally ambiguous human-feeling replies. The aim is for the user to question what kind of voice they are interacting with, rather than treating the chatbot as a neutral interface.

- Website: https://yze.design/tamagotchu/
- Process: https://yze.design/tamagotchu/process/
- Repository: https://github.com/yze1/tamagotchu

## Contents

- `index.html` - main page structure.
- `style.css` - retro screen layout, wrapper styling, and visual effects.
- `scripts/video.js` - button-controlled intro/left/right video states.
- `scripts/script.js` - RiveScript loading and chat message handling.
- `scripts/score.js` - counter interaction.
- `brain/` - RiveScript triggers, topics, substitutions, and response sets.
- `media/` - background and interaction videos.
- `wrapper-media/` - scanline, overlay, and screen wrapper assets.

## Run

Serve the folder locally:

```bash
python3 -m http.server 5500
```

Open `http://127.0.0.1:5500/`.

Click the top control to play the introduction, use the left/right controls for video responses, and type into the chat field to talk to Gotchu.

## Git Notes

Large media assets are tracked with Git LFS. Run `git lfs pull` after cloning if videos or images are missing.
