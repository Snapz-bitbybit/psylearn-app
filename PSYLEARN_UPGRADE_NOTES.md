# PSYLEARN Improved Version Notes

This rebuilt version keeps the original PSYLEARN identity but improves the learning flow and academic strength.

## Main upgrades

1. Quiz timer logic fixed
   - The memorizing mode timer now uses `useEffect` instead of `useState`.
   - This prevents repeated interval bugs.

2. Memorizing mode improved
   - Explanation now appears after each answer, including memorizing mode.
   - Learners still receive fast feedback, but the explanation supports actual learning.

3. Score calculation fixed
   - Answers are recorded once only.
   - Final result uses the stored answer list to avoid double-counting.

4. Result page upgraded
   - Added Performance Level: Foundation, Developing, Advanced.
   - Added Suggested Next Step.
   - Button label changed to `Back to Dashboard` so the navigation matches the actual function.

5. Learning experience upgraded
   - Added live progress, current score, mode label, and learning tips.
   - The quiz now feels closer to NotebookLM-style guided feedback.

## Recommended academic explanation

PSYLEARN can be presented as a psychology learning quiz app that combines:

- Retrieval practice through quizzes
- Immediate explanatory feedback after answers
- Gamification through XP and progress indicators
- Metacognition through journal reflection
- Learning preference awareness through VARK assessment
- Working memory training through the memory game

## Suggested future upgrade

The next strongest improvement would be connecting VARK results to personalized recommendations, such as:

- Visual learner: recommend notes and diagrams
- Auditory learner: recommend explanation/audio mode
- Reading/Writing learner: recommend notes and journal
- Kinesthetic learner: recommend quiz and memory game
