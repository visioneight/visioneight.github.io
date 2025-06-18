#### 1. **Navigation Flow Set Up**
- Connected screens in this order: `StartScreen` → `TutorialScreen` → `PracticeScreen` → `TestScreen`.
- Fixed bug where the second “OK” in the tutorial skipped the practice screen.
- Used `Navigator.pushReplacementNamed()` for clean screen transitions.

#### 2. **Practice Screen UI Implementation**
- Designed and implemented a new interface where users tap areas based on arrow direction.
- Divided the screen into four directional zones:
  - Left: light grey
  - Up: dark grey
  - Right: semi-transparent blue
  - Down: semi-transparent red
- Center arrow (SVG) displayed and rotated accordingly.
- “I’m Ready” button added to transition into the actual vision test.

#### 3. **Test Logic & Screen Refactor**
- Replaced old “I see it / I don’t see it” buttons with directional input.
- Arrow direction is randomized.
- Vision level logic:
  - Each level (defined by decreasing arrow size) has 5 trials.
  - If the user gets at least 3 correct → proceed to next level.
  - Otherwise → test ends. (Possibly change this to 2 fails -> decrease difficulty)
- Background areas are interactive via `GestureDetector`.

#### 4. **Next Steps / TODO**
- Implement left-eye and right-eye test transitions.
- Add result summary screen after test ends.
- Decide on storing user data or visual stats.
- Implement depth estimation.
