> **Archived.** 2024 experiment by FRC Team 6907; not maintained. A Roboflow API key that used to be hard-coded in this README has been removed from this file. It is still in the git history, so it must be treated as compromised.

# FRC-Game-Piece-Detection
Game Piece Detection with Roboflow dataset and YOLO model

### Dataset Usage
!pip install roboflow

from roboflow import Roboflow
rf = Roboflow(api_key="YOUR_ROBOFLOW_API_KEY")
project = rf.workspace("frc-3707").project("2024-game-piece")
version = project.version(2)
dataset = version.download("yolov8")
