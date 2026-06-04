- [ ] Inspect `src/model/hybrid_model.py` (and any related explainer/schema) to see how component scores are produced.
- [ ] Implement `explanation` generation inside `HybridRecommender.recommend(..., explain=True)` based on the dominant contributor (content vs collab vs sentiment).
- [ ] Ensure API pass-through: `GET /api/recommend` and websocket `/ws/recommendations` include `explanation` in each recommendation object.
- [ ] Update `frontend/app.js` to render `r.explanation` under each recommendation card for both HTTP and websocket flows.
- [ ] Add/adjust tests for `explain=True` output shape (if the repo has tests covering `recommend`/hybrid outputs).
- [ ] Run `pytest` and any frontend checks; do a quick manual verification of the UI.

