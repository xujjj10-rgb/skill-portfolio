# Interaction states

## Album

Track `displayedIndex`, `requestedIndex` and a request token separately. Decode the destination photograph and its sticker assets before replacing the visible page. Only the latest request may commit. A failed request leaves the previous photo visible and offers a retry.

Reserve portrait/landscape space based on the media. Keep the toolbar outside the independently scrolling photo area so large images remain large without forcing visitors to find the controls. Change only that pane's scroll position on page change.

Retain button and arrow-key navigation. Confine optional horizontal swiping to the photo area, ignore mostly vertical gestures and screen-edge starts, and preserve pinch zoom and page scrolling. No automatic slideshow unless requested.

On completion, announce the actual displayed page, not only the requested one. Check first/last boundaries and fast changes to nonadjacent pages.

## Gift box

Use `wrapped → opening → revealed`. Apply immediate pressed feedback, then a short ribbon/lid transition. Ignore duplicate activation while opening. At completion expose the real gift and move focus only if the dialog is still open and the same gift remains selected.

Closing the dialog or selecting another gift must resolve the in-flight transition. Choose either cancel-and-return-to-wrapped or finish-and-remember; use it consistently. Never let a delayed callback change a closed dialog or steal focus.

Distinguish "gift revealed" from "gift switched on". An opened humidifier may remain switched off; a revealed mug need not be filled yet. Label those actions separately.

Remember opened gifts only at the persistence level the task calls for. Session storage means this tab/session, not permanent memory. A replay action must clearly state which states it resets.

## Modal and scene return

Use an accessible dialog with a visible close button and Escape support. Keep the return location predictable. Do not layer multiple modal dialogs accidentally. Restore focus to a sensible trigger after closing, especially if a loading control disappeared during a reveal.

## Behavioral checks

1. Open an album at its first photo; request a middle page and immediately request the last. Last request wins.
2. Simulate a missing photo: previous page remains visible and navigation remains usable.
3. Start opening a gift and close the dialog before completion. Reopen: the state is coherent and focus stays in the active view.
4. Reopen a revealed gift: it does not accidentally replay the reveal or reset another gift.
5. With reduced motion enabled, perform the same actions without depending on animation completion.
6. Use keyboard and a small phone layout; ensure fixed controls do not cover photos or focused buttons.
