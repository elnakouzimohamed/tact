# T.A.C.T — Tactical Augmented Coaching Translator

**T.A.C.T**, short for **Tactical Augmented Coaching Translator**, is an AI- and AR-powered basketball training system designed to bridge the gap between how basketball tactics are explained and how they are executed on court.

> This repository is a public overview of the project.  
> The source code is private and not included in this repository.

## Demo Video

Watch the project demo here:  
https://youtu.be/rNGbi9OeANU?si=NVREzw0GbWTXKD8e

## Project Overview

Basketball academies and young trainees often struggle to understand complex tactic-board drawings and convert them into real on-court movement. T.A.C.T addresses this problem by transforming a coach’s 2D tactical explanation into an interactive augmented reality training scenario.

The system allows a coach to upload or record a video explanation on a tactical board. An AI-based analysis pipeline then extracts the players, positions, timing, and basketball actions into a structured JSON format. This structured output is executed in Unity, where each action is mapped to animation clips and synchronized with virtual players in a 5v5 training simulation.

## Core Features

- AI-based analysis of coach tactic-board explanations
- Conversion of tactical videos into structured JSON plays
- Unity-based 5v5 basketball simulation
- Augmented reality visualization of tactics
- Real-court and virtual-court training modes
- Persistent AR court placement using spatial anchoring
- Manual court calibration for real-world alignment
- Rover-based computer vision feedback system
- Player tracking and action verification
- Pose-based free-throw form analysis
- Performance feedback for positioning, passing, shooting, and receiving

## System Pipeline

The T.A.C.T workflow follows this pipeline:

1. **Coach Input**  
   The coach records or uploads a video explaining a basketball tactic on a 2D tactic board.

2. **AI Analysis**  
   The video is processed using AI to extract the players, positions, action timing, and basketball movements.

3. **JSON Generation**  
   The extracted tactical information is converted into a structured JSON format.

4. **Unity Execution**  
   Unity reads the JSON output and maps each action to synchronized player animations.

5. **AR Training Scene**  
   The play is visualized in augmented reality, allowing trainees to understand their roles in a more immersive way.

6. **Computer Vision Feedback**  
   A rover-based vision system tracks the player and supports real-time feedback on action execution and movement quality.

## Real-Time Feedback System

A key contribution of T.A.C.T is closing the training loop through feedback. The system uses a rover equipped with a Raspberry Pi and camera to track the trainee during practice. Through WebSocket communication, the rover sends visual feedback data to the training system.

The computer vision module supports:

- Player tracking
- Position verification
- Passing action feedback
- Shooting action feedback
- Receiving action feedback
- Posture and movement analysis

## Free-Throw Training Module

T.A.C.T also includes a free-throw training module that uses pose estimation to evaluate shooting form. The system analyzes body posture, detects key movement patterns, and generates performance feedback to help players improve their shooting mechanics.

## Technologies Used

- Unity
- Augmented Reality
- Artificial Intelligence
- Computer Vision
- Pose Estimation
- Robotics
- Raspberry Pi
- WebSocket Communication
- JSON-based play representation
- Spatial Anchoring
- Court Calibration

## Project Status

T.A.C.T is currently a closed-source academic engineering project. This repository is intended to provide a public overview of the project, its purpose, system architecture, and demo video.

The implementation code, backend logic, AI prompts, Unity scripts, and rover control modules are not publicly available.

## Authors

Developed as part of an engineering project.

## License

This repository is for informational and portfolio purposes only.  
All project rights are reserved. No source code is provided or licensed for reuse.
