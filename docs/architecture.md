# Real2Sim Architecture

## System flow

Real-world sensors -> perception -> structured scene -> simulation -> evaluation -> candidate fix -> human approval -> controlled deployment.

## Workstreams

### Robotics + Real2Sim
Owns robot interfaces, ROS 2 integration, real-world logging, controller interfaces, and real-to-simulation integration.

### Perception + Scene Extraction
Owns camera/calibration pipelines, scene extraction, scene representation validation, and perception evaluation.

### Backend + Dashboard + AI Orchestration
Owns experiment APIs, persistence, dashboard, run orchestration, AI-assisted analysis, and approval records.

### Simulation
Provides reproducible scenes, variations, benchmark definitions, and simulation runners shared by all workstreams.

## Safety boundary

AI may propose changes, but candidate changes remain isolated and simulation-tested until a human approves deployment to hardware.
