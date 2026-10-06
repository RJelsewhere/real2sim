# Contributing

## Team ownership

- **Robotics + Real2Sim:** `robotics/`
- **Perception + Scene Extraction:** `perception/`
- **Backend + Dashboard + AI Orchestration:** `backend/`

Shared work lives in `docs/`, `simulation/`, and `tests/`.

## Workflow

1. Create a focused branch from `main`.
2. Keep commits small and descriptive.
3. Add or update tests for behavior that changes.
4. Document changes to shared contracts in `docs/contracts/`.
5. Open a pull request for review.
6. Do not deploy AI-generated changes to physical hardware without human approval.

## Shared interfaces

Changes to JSON contracts should be reviewed by all affected workstreams. Prefer backward-compatible additions when practical.

## Pull requests

Every PR should explain:
- What changed
- Why it changed
- How it was tested
- Whether a shared contract changed
- Whether simulation validation was performed

## Safety

AI-generated patches must remain isolated until they have passed simulation testing. Human approval is required before hardware deployment.
