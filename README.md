# 💖 The Ultimate Interactive Romantic Apology & Date Invitation

A playful, funny, dramatic, and heartfelt interactive apology website inspired by **iamreallysorry.com**. Built with **Next.js (App Router)**, **React 19**, **TypeScript**, and **Tailwind CSS**.

---

## 🌟 The Experience Flow

1. **Stage 1: The Dramatic Opening**
   - Floating whimsical pastel emojis, clouds, and stars.
   - Giant glossy 3D beating heart with realistic lub-dub pulse.
   - Click the heart to feel the heartbeat sound and trigger bursting mini-heart particles.
   - Playful teaser: *"Someone has messed up big time. And that someone is me."*
   - Personalized greeting: *"Hey [GIRLFRIEND_NAME] ❤️"*
   - Smooth transition button to jump right into the apology.

2. **Stage 2: The Apology Meter ("HOW SORRY AM I?")**
   - Animated sorry meter that rapidly climbs: `0%` → `100%` → `250%` → `500%` → `1000%`!
   - Visually overflows its boundary with glowing flames and alarm buzzer.
   - Flashing banner: *"WARNING: SORRY LEVELS EXCEEDING SAFE LIMITS 🚨"*
   - Sincere, honest apology letter acknowledging her disappointment about missing the concert with zero excuses.
   - 3 interactive cards: *"MY BAD"*, *"YOUR FEELINGS MATTER"*, and *"LESS TALK, MORE ACTION"*.

3. **Stage 3: The Funny Interlude**
   - *"Things I should have done differently..."*
   - Humorous cards:
     1. Leave earlier.
     2. Stop pretending I have unlimited time.
     3. Check the time approximately 47 times.
     4. Actually respect concert timings.
     5. Not make my girlfriend miss a concert.
   - Embarrassed reaction badge: *"Yeah... I know. I deserve that look. 😭"*

4. **Stage 4: The Big Invitation & Runaway NO Button**
   - *"Can I take you out tonight?"*
   - **YES Button (`YES, LET'S GO! 💗`)**: Bright, glossy hot pink, with a gentle bounce and soft glow. As the NO button is chased, the YES button progressively grows larger and more tempting!
   - **Runaway NO Button (`NO 😤`)**:
     - **Desktop**: Cursor proximity detection moves the button away when the mouse approaches within 65px.
     - **Mobile**: Touch detection triggers an escape jump on tap.
     - **Progressive Shrink**: Shrinks from 100% → 90% → 80% → 70% → 60% → 50% → 42% (min 42%).
     - **Funny Speech Bubbles**: Cycles through hilarious remarks (*"HEYYY, WAIT! 😭"*, *"Are you really saying no?"*, *"LOOK HOW SMALL IT'S GETTING 😭"*).
     - **Cartoon Sound Effect**: Playful boing sound on every escape.
   - **Respectful Alternative Link**: Fixed, non-moving link (*"Not tonight — I need some time."*) honoring her genuine feelings with a warm, zero-pressure message.

5. **Stage 5: The Celebration**
   - Triggered when **YES** is clicked.
   - Full-screen multi-stage confetti explosion with `canvas-confetti`.
   - Romantic chime and celebratory fanfare.
   - *"WHAAAAAT?! SHE SAID YESSSSS!!! 🥹❤️"*

6. **Stage 6: The Date Night Reveal**
   - Digital VIP Date-Night Pass for tonight:
     - 01 — DINNER 🍝
     - 02 — A LITTLE WALK 🌃
     - 03 — SOMETHING SWEET 🍰
   - Copy evening plan button with one-click clipboard copying.
   - *"PS: This time, I am leaving early. Very early. Unnecessarily early. 😭"*

7. **Stage 7: Respectful Decline**
   - Sincere, pressure-free reassurance if she selects *"Not tonight"*.

8. **Audio & Sound System**
   - Corner floating control: `🎵 MUSIC OFF` / `🎵 MUSIC ON` with smooth fade-in/fade-out.
   - Synthesized Web Audio sound effects (heartbeats, boing, meter alarm, chimes, pops).
   - Independent `SFX ON` / `SFX OFF` toggle.
   - **Off by default** until the user interacts.

---

## ✏️ How to Personalize

All personalization is managed in a single file: **[`src/data/siteConfig.ts`](file:///c:/Users/deepa/OneDrive/Desktop/leeja/src/data/siteConfig.ts)**.

Simply edit your names, dates, or restaurant/walk spots:

```typescript
export const siteConfig = {
  boyfriendName: "YourName",       // Replace with your name
  girlfriendName: "HerName",       // Replace with her name

  // Edit itinerary details
  celebration: {
    itinerary: [
      {
        number: "01",
        title: "DINNER",
        emoji: "🍝",
        location: "[FAVORITE RESTAURANT]", // e.g. Bella Vista
        time: "7:30 PM",
        description: "Cozy table, zero rush, and all your favorite food."
      },
      ...
    ]
  }
};
```

---

## 🚀 Running the App

```bash
# The server is currently active on:
http://localhost:3000
```
