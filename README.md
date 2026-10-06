# Real2Sim

A 3-person research and engineering project for building a Real2Sim pipeline that connects real-world observations, scene reconstruction, simulation, evaluation, and controlled deployment.

## Project goals

- Capture and log real-world robot/perception data.
- Extract structured scene representations from sensor data.
- Reconstruct and vary simulation scenes from real observations.
- Run reproducible simulation benchmarks.
- Provide backend orchestration and a dashboard for experiments.
- Use AI to propose fixes while keeping human approval in the deployment loop.

## Team areas

1. **Robotics + Real2Sim** — ROS 2 integration, robot control, logging, and real-to-simulation interfaces.
2. **Perception + Scene Extraction** — camera/calibration pipelines, scene extraction, and validation.
3. **Backend + Dashboard + AI Orchestration** — APIs, data storage, experiment dashboard, and AI workflow orchestration.

## Safety boundary

AI-generated patches must be isolated and simulation-tested before they can be considered for hardware deployment. Human approval is required before deployment to physical hardware.

## Repository layout

```text
robotics/       Robot and Real2Sim integration
perception/     Perception, calibration, and scene extraction
backend/        APIs, database, dashboard, and AI orchestration
simulation/     Scenes, variations, benchmarks, and runners
docs/           Architecture, contracts, and project planning
tests/          Cross-component tests
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for the development workflow.
