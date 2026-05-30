# Zivon Voice UI

Voice interface preview for the Zivon AI orchestration system. Four conversation states — Idle, Listening, Thinking, Responding — each driven by a short looping animation.

## Versions

| Version | Path | Notes |
|---------|------|-------|
| v1 | [`v1/`](v1) | Frozen baseline. Idle 1s, Listening 2.5s, Thinking 2.5s, Responding 2.2s. State-pure clips with fade-out/fade-in swaps so no other state is glimpsed during transitions. |
| v2 | [`v2/`](v2) | Working copy for new iterations. |

## Run locally

```bash
cd v1   # or v2
python3 -m http.server 8765
# open http://localhost:8765/preview.html
```

## Files

Each version contains:
- `preview.html` — the 4-button preview UI
- `0_idle.mp4`, `1_listening.mp4`, `2_thinking.mp4`, `3_responding.mp4` — state clips
