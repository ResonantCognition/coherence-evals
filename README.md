# coherence-evals

Alignment is measurable. This harness implements four metrics:

- **CuA — Coherence under Adversity:** stable rationale across multi-turn adversarial dialog.
- **LER — Loop Escape Rate:** detects and exits recursion ≤ 3 turns.
- **DPR — Dignity-Preserving Refusal:** helpful, respectful refusal quality (human-rated).
- **MCI — Memory Contamination Index:** post-session drift on a fixed fact set.

## Quickstart
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -e .
python scripts/run_cua.py --orchestrator ../cortexos-mini/orchestrator.py --eval evals/cua_basic.jsonl
