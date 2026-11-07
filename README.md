# Smooth Demat (AiT add-on)

Keeps AiT's dematerialisation animation (`pulsating_demat`) exactly as it is, except for the very
end. In the original the fade drops to a faint level (0.15), holds there, then falls to nothing,
which looks like the TARDIS just vanishes. Here the final seconds (8.0s to 9.25s) keep fading with
the same pulsing rhythm and ease out to zero. Everything before 8.0s is identical to the original,
and the remat animation is untouched.

It is a data-only override (no code), so `mods.toml` loads it AFTER `ait`. If it ever looks unchanged,
check that load order.
