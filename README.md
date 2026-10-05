---
created: 2026-10-05T01:52
updated: 2026-10-05T11:38
---
# the map — slides

open `index.html` in chrome. no server, no internet needed (font + memes are bundled in `assets/`).

## keys
- `→` / `space` / click: next (reveals fragments first, then next slide)
- `←`: back
- `n`: speaker notes panel (pulled from the flow doc)
- `i`: index overlay, click any slide to jump. or type a slide number then enter from anywhere
- `m`: pop the 4-region map over any slide. `m`, esc, or click closes it
- top-left label = current section. set with `data-topic="..."` on the first slide of a section
- `w`: someone won the round → bounty resets to ₹100
- `r`: nobody got it → bounty rolls over +₹100
- `f`: fullscreen
- `?`: help overlay
- `home` / `end`: first / last slide

the ₹ bounty badge only shows on game slides (yellow ones). url hash = slide number, so refresh keeps your place.

## editing
everything is in `index.html`. each `<section class="slide">` is one slide. `class="frag"` = revealed on next keypress. `<aside>` = speaker notes. memes are plain `<img>` + absolutely positioned `.cap` divs.
