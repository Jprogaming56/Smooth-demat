# Smooth Demat (AiT add-on)

Personal add-on for Adventures in Time (AIT Forger), Forge 1.20.1. Not for sharing.

Replaces the default dematerialisation animation (AiT's `pulsating_demat`) with a smoother one.

What was wrong: the original fade drops to a faint level, holds there, then falls to nothing in
the last second, and its flicker is made of only a few jumpy keyframes, so the ending looks like
the TARDIS just vanishes.

What this does: same length and same start (it stays solid for the first 1.5 seconds, so the demat
sound and the take-off still line up). After that it fades along a smooth curve that eases out and
reaches zero gently at the very end, with soft pulses that swell and then die away before the end
instead of cutting off. The materialisation animation is left exactly as it was.

It is a data replacement only (no code): `data/ait/fx/animation/keyframes/pulsating.animation.json`.
The mod loads after AiT so its file wins. Other demat animations (classic, drill and so on) are
untouched. Remove the mod to go back to the original.
