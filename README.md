# Player Tracking & Re-Identification using YOLOv8 + Norfair

This project performs player tracking and re-identification in a video using YOLOv8 and Norfair.

## How it works
- Uses **YOLOv8** to detect players frame-by-frame.
- **Norfair Tracker** assigns consistent IDs even when players move out and re-enter the frame.
- Output is a video with bounding boxes and consistent IDs, plus a match timer overlay.

## Files Included
- `15sec_input_720p.mp4`: Sample input video
- `Players_TrackingCode.ipynb`: Code notebook
- `player_tracking_output.mp4`: Final annotated video output
- `tracking_log.csv`: CSV log of ID positions per frame

## How to Run
1. Open the `.ipynb` file in Google Colab.
2. Upload your video when prompted.
3. The code will:
   - Extract frames
   - Run detection + tracking
   - Annotate and save output video
4. Downloads output video and CSV automatically.

## Dependencies
- Python 3.8+
- OpenCV
- Ultralytics YOLOv8
- Norfair
- Pandas, NumPy

## Notes
- Works best with videos where people are clearly visible.
- Tracking IDs remain consistent even if individuals go out of frame.
