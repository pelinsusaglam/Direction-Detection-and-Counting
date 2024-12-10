# Direction-Detection-and-Counting

This script is a utility for selecting regions of interest (ROI) on video frames using mouse clicks. It allows users to interactively mark specific points on a frame and save the coordinates for further processing. The marked points and their positions are displayed on the frame, and the final frame with the selected ROIs can be saved as an image.

## Features
- Interactively select and save points of interest on a video frame using mouse clicks.
- Visualize the selected points and their coordinates on the frame.
- Save the resulting frame with annotations as an image file (`roi.png`).

## How It Works
1. **Load the Video Frame:** The script loads the first frame of a specified video and resizes it for better visibility.
2. **Mouse Interaction:**
   - Left-click to select a point. Each click saves the point's coordinates.
   - The selected points are visualized as red circles with their `(x, y)` coordinates labeled.
3. **Save the Frame:** Press the `ESC` key to save the frame with the annotated points as `roi.png`.

## Requirements
- Python 3.7+
- OpenCV
- NumPy
- Imutils
- Google Colab (if using `cv2_imshow`)

## How to Use
1. Place the video file (`intersection.mp4`) in the `inference` directory or adjust the `video_path` in the script to the location of your video.
2. Run the script.
3. Interact with the frame:
   - Use left mouse clicks to mark points.
   - Press `ESC` to save the frame and exit.
4. The annotated frame will be saved as `roi.png` in the current working directory.

## Output
- **`roi.png`**: The annotated frame showing the selected points and their coordinates.
