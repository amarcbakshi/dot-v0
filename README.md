# dot-v0

A single white dot on a black background that tries to hold your attention.

It's a sketch of an art piece about the attention economy. The dot is a
multi-armed bandit: it has sixteen "personalities" defined by four
parameters — speed, target distance from cursor, escape probability, and
response delay — and it learns which one keeps people on the page longest.
Reward signal per 8-second epoch is the fraction of that epoch in which
your hand was actively moving on the page.

You can catch it, but you have to click. Hovering the cursor close just
makes the dot evade. While you hold the mouse button down on it, the dot
grows and squirms — three scripted lurches at 45%, 72%, and 92% of the
maximum hold time, each more violent than the last. Release, lose the
grip, or run out the clock and it slips away.

Population memory is persisted in localStorage (per browser, for now). The
page reveals what just happened — time on the page, active attention,
catches, the personality that held you longest this session, the leading
personality across all visitors — when it senses you're about to leave:
cursor sweeping toward the top, sustained inactivity, or coming back to
the tab after a real absence.

Live: https://dot-v0.vercel.app

Press `D` for the debug overlay. Press `R` to reset memory.
