🦾 BoraFlow AI: High-Velocity Kinetic Signature Recognition
BoraFlow AI is an end-to-end deep learning pipeline designed to recognize and classify complex human motion sequences in real-time. By leveraging a Stacked LSTM architecture and MediaPipe pose estimation, the system identifies intricate choreographies with high precision, specifically optimized for high-velocity transitions.

<img width="1232" height="606" alt="image" src="https://github.com/user-attachments/assets/4446e029-92d5-4e94-bbbc-43479b4fd9f2" />

🚀 Key Performance Metrics

Real-Time Confidence: 87.90% (on 'ON' Choreography)

Validation Accuracy: ~96% (across 16 classes)

Inference Speed: ~59.3ms per sequence

Dataset Scale: 16 classes | 85,000+ frames of kinetic data

🧠 The Architecture

The project utilizes a hybrid Computer Vision and Recurrent Neural Network (RNN) approach:

Detection: YOLOv11 for robust human subject localization.

Keypoint Extraction: MediaPipe Pose for extracting 33 3D-landmark coordinates.

Temporal Processing: A Stacked LSTM (Long Short-Term Memory) network to capture the "rhythm" and temporal signatures of movement over 30-frame windows.

📉 The Iteration (Engineering Honesty)

This project was built on the principle of data-driven iteration.

Phase 1: Initial training on 11 classes yielded a 70.3% confidence score on real-time inference.

Phase 2 (Scaling): The dataset was expanded to 16 classes, adding high-velocity choreographies (including IDOL, Dynamite, Butter, and ON).

Result: The increased spatial variety in the dataset allowed the model to better distinguish complex joint isolations, pushing the real-time confidence for the 'ON' class to 87.90%.

<img width="773" height="602" alt="image" src="https://github.com/user-attachments/assets/424dfe34-ce62-4307-bd0f-7a7e10bc3726" />

🛠️ Tech Stack
Language: Python

Deep Learning: TensorFlow / Keras

Computer Vision: OpenCV, MediaPipe, YOLOv11

Data Manipulation: Pandas, NumPy

Visualization: Matplotlib

Data Manipulation: Pandas, NumPy

Visualization: Matplotlib
