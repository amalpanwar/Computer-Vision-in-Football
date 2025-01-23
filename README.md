# Computer-Vision-in-Football
# Football Video Analysis with AI

## Overview
This project leverages advanced AI models and computer vision techniques to analyze football match videos. The system detects, tracks, and annotates players, evaluates their performance, and provides valuable insights for tactical analysis. The primary objectives are to:

1. Detect and track players using YOLO and ByteTrack.
2. Predict teams based on jersey color using a custom ML algorithm.
3. Annotate videos with player speed, distance covered, and real-life pitch positions.
4. Generate a comprehensive dataset in CSV format for further analysis of match events and strategies.

---

## Features
- **Object Detection**: Utilizes YOLO for accurate player and ball detection.
- **Object Tracking**: Tracks player movements with ByteTrack to maintain consistency.
- **Team Classification**: Predicts team affiliations using jersey color.
- **Annotation**: Displays speed, distance, and player positions on a virtual pitch.
- **Homography Transformation**: Maps video coordinates to real-life pitch dimensions.
- **Automated Data Generation**: Saves annotated data, including speed, position, and timestamps, to CSV files.
- **Tactical Analysis**: Supports deep insights into defensive and attacking strategies by analyzing key match events.

---

## Technologies Used
- **Python**
- **YOLO (You Only Look Once)** for object detection
- **ByteTrack** for multi-object tracking
- **OpenCV** for image processing and video analysis
- **Numpy & Pandas** for data handling and processing
- **Matplotlib** for data visualization and annotations

---

## Sample Annotation
Below is a sample image demonstrating the annotated output:

![Annotated Football Pitch](Sample_annotated.png)

- Black circles: **Elgin City players**
- Red circles: **Bonnyrigg Rose players**
- Yellow circle: **Refree**
  

---

## How It Works
1. **Object Detection and Tracking**
   - YOLO detects players, ball, and other objects in each video frame.
   - ByteTrack ensures players are tracked seamlessly across frames.

2. **Team Classification**
   - A machine learning model predicts team affiliation based on jersey color.

3. **Homography Transformation**
   - Maps detected coordinates to real-life pitch dimensions, allowing accurate player positioning.

4. **Annotation and Visualization**
   - Annotates frames with player IDs, timestamps, speed, distance covered, and pass directions.

5. **Data Storage**
   - Extracted data is saved in CSV files, which can be analyzed to review specific match events or timestamps.

---

## Challenges
- **Non-Official Camera Setup**: Some manual adjustments were necessary due to irregularities in non-professional recordings.
- **AI Limitations**: Occasional misclassifications were mitigated with manual intervention.

---

## Results
- Automated data generation with **89% MAPE precision**.
- Comprehensive match analysis available in CSV format.
- Scalable and customizable for different match scenarios.

---

## Usage
1. Place the video file in the `videos/` directory.
2. Run the script to analyze the video and generate CSV files.
3. Visualize annotated frames using the Matplotlib script provided.

---

## Future Enhancements
- Improve detection accuracy for low-quality videos.
- Incorporate advanced analytics like heatmaps and possession statistics.
- Extend compatibility for other sports.

---

## Contributions
Contributions are welcome! Feel free to open issues or submit pull requests.

---

## License
This project is licensed under the MIT License.

---

## Contact
For any queries, please reach out to [your_email@example.com].

