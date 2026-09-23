# T-001 Task Prompt

- Task ID: T-001
- Stage: MVP demonstration
- Owner: Codex
- Approver: User
- Dependencies: 無
- Goal: Repair the 《山居秋暝》 per-character Jyutping exercise.
- Scope: `versions/article/index.html` plus acceptance evidence in `PROJECT_LEDGER.md`.
- Inputs: Existing eight-line, 40-character poem data and the current screenshot-inspired layout.
- Outputs: One input per poem line, Enter-based answer checking and advancement, feedback, completion, and restart.
- Acceptance evidence: JavaScript syntax check and reproducible checks for correct Enter, wrong answer, line transition, final character, and restart.
- Assumptions: Punctuation is not answered; Jyutping tone digits are significant; a wrong answer displays the correct Jyutping and leaves the current character selected.
- Unresolved decisions: None.

## 必須做
- Keep the poem visible with one wide input per line and only enable the line containing the current character.
- On correct Enter, immediately advance exactly one character and focus the active line input.
- On incorrect Enter, stay on the current character and show its expected Jyutping.
- Show completion after all 40 characters and allow restarting with score/results reset.
- Verify the listed acceptance behaviors.

## 不能做
- Do not change the other learning features, poem content, or version navigation.
- Do not accept a Jyutping answer with an incorrect tone number.
- Do not leave event handlers referring to removed elements.

## 正向例子
- Entering `hung1` for `空` marks it correct and focuses the input for `山`.
- Entering an incorrect answer for `空` keeps `空` current and displays `hung1`.

## 負向例子
- A detached confirmation button or Enter handler that does nothing.
- Accepting `hung2` as correct for `空`.
- Advancing after an incorrect answer or stopping before restart can be tested.
