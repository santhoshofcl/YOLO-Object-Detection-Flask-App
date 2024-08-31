# YOLO-Object-Detection-Flask-App
This project provides a web application that uses YOLO (You Only Look Once) for real-time object detection. The application captures live video from your webcam, processes the frames using YOLO, and displays the video stream with detected objects annotated with bounding boxes and labels.
Here's a sample `README.md` file for your Flask-based YOLO object detection web app:

## Requirements

- Python 3.x
- Flask
- OpenCV
- Numpy

## Installation

1. **Clone the repository**:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Create a virtual environment** (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Download YOLO files**:

   - `yolov3.weights`
   - `yolov3.cfg`
   - `coco.names`
     
   Place these files in the same directory as your script or update the file paths in `app.py`.

## Running the Application

1. **Start the Flask application**:

   ```bash
   python app.py
   ```

2. **Access the web application**:

   Open a web browser and navigate to `http://127.0.0.1:5000/` to view the video feed with object detection annotations.

## Code Explanation

- **`app.py`**: Main application file containing Flask routes and YOLO object detection logic.
  - `/`: Renders the HTML page with the video feed.
  - `/video_feed`: Provides the video stream with YOLO object detection applied.

- **`index.html`**: Basic HTML page to display the video stream. Ensure this file is located in the `templates` folder.

## Troubleshooting

- **Camera Not Working**: Ensure your webcam is properly connected and not being used by another application.
- **File Not Found**: Verify that the paths to `yolov3.weights`, `yolov3.cfg`, and `coco.names` are correct.
- **Dependencies Issues**: Make sure all dependencies are installed and up-to-date.
