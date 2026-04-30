## What I did
- Ran all existing test files in the VM and documented results
- Wrote a full `TESTING_PLAN.md` covering unit, integration, system and UAT
- Wrote Gherkin scenarios for each feature

## Test results

| Test | Result |
|------|--------|
| `test_tts.py` — TTS engine | PASS |
| `test_ollama.py` — Ollama connection | PASS (after model name fix) |
| `test_model.py` — Granite response | PASS — 1.3s |
| `main.py` mock mode | PASS |
| Engineer Q&A | PASS |
| `novice_wrapper.py` mock | PASS |
| `livery_wrapper.py` | PASS |

## Blockers
- VM had broken venv — paths hardcoded to a different machine
- `pip` wouldn't run through the venv

## Fixed by
- Used system Python directly: `C:\Users\r.d.a\AppData\Local\Python\bin\python.exe`
- All packages installed cleanly via `pip install -r requirements.txt`

