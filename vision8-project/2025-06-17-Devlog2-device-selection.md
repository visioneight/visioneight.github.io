# Devlog – June 17, 2025

## App Logo

![Vision8 App Logo](/image/app_logo.jpeg)

## Company Logo

![Company Logo](/image/company_logo.png)

---

## What I Did
- Refactored the visual acuity test flow in the Vision8 app:
  - Added a convergence condition based on re-entry into the same test level (stabilization logic).
  - Test terminates if the same level is re-entered twice, or if the user gets 3 correct answers at that level.
- Simplified test progression logic to avoid infinite loops in edge cases.
- Converted millimeter sizes to pixels using a factor of `3.7795`, assuming 96 DPI screen.
- Added a gamelike tutorial test to ensure the user is familiar with the interface.

## What I Learned
- Re-entry-based stabilization is more user-friendly and effective than just correctness thresholds.
- Premature test termination can be avoided by balancing progression conditions.

## What's Left / Next Steps
- Implement distance-based scaling: dynamically adjust SVG size using viewing distance and screen DPI.
- Add logic that estimates depth through image provided (This will include image recognition).
- Add prompts and logic for left-eye and right-eye separation.
- Finalize post-test result display with timestamp, eye-specific acuity as a chart.
- User needs to answer checklists which will help them diagnose possible functional degradation of eyesight.
