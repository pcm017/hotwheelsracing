# Hot Wheels Race Timer

A phone-camera finish-line timer for Hot Wheels (or any small-scale) races. Point your phone at the track, draw a box over the finish line, and the app watches for motion in that zone to automatically clock each run — no button-mashing required.

**[Use it now →](https://pcm017.github.io/hotwheelsracing/)** (or open `index.html` yourself, see below)

## How it works

1. Tap **CAM ON** and allow camera access — it uses your phone's rear camera by default so you can point it straight at the track (tap the 🔄 button to switch to the front camera if you've mounted your phone differently).
2. Drag a box over the finish line to set the **finish zone**.
3. Type a car name, hit **start**, and let it go — when motion crosses the zone, the timer stops automatically, with confetti and a sportscaster-style announcer call.
4. Run multiple cars/heats and see a live leaderboard.

Everything runs entirely in the browser — no server, no accounts, no data leaves your device.

## Running it yourself

No build step, no dependencies. Either:

- Use the hosted version above, or
- Clone this repo and open `index.html` directly on your phone (Chrome/Safari), or
- Serve it locally (camera access requires HTTPS or localhost, not `file://`):
  ```
  python -m http.server 8080
  ```
  then visit `http://localhost:8080` on your phone (same Wi-Fi network).

## Optional: announcer voice

By default, finish/podium calls use your browser's built-in text-to-speech. For a higher-quality announcer voice, you can enter your own [ElevenLabs](https://elevenlabs.io/) API key in the app's settings — it's stored only in your browser's local storage and is never sent anywhere but ElevenLabs' API. This is entirely optional.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, run your own races with it.
