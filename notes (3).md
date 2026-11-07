# Assignment 6.4 - Notes

- **Sticky navbar:** `.navbar { position: sticky; top: 0; z-index: 100; }` scrolls with the page until it reaches the top, then stays there.
- **Fixed button:** `.help-btn { position: fixed; right: 24px; bottom: 24px; z-index: 200; }` stays in the bottom-right corner of the viewport at all times.
- **Absolute badge:** `.badge { position: absolute; top: -10px; right: 12px; }` is placed relative to its card because `.card { position: relative; }` is the nearest positioned ancestor. Without `position: relative` on the card, the badge would jump to the page corner.
- **z-index order:** help button (200) > navbar (100) > badges (1) > normal content. Scrolling cards pass under the navbar, and the help button always stays on top.

## Screenshot (to take yourself)
Scroll until the "Featured hikes" cards are just below the navbar, then capture the window so that the sticky navbar, the orange help button and at least one badge are visible. Optionally label them with arrows.
