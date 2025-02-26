# Coffee Drinking Detection

This project detects when a person is drinking coffee using OpenCV and plays a sound alert using Pygame.

## Requirements

Ensure you have the following dependencies installed:

```sh
pip install opencv-python numpy pygame
```

## How It Works

1. **Face Detection**: The program uses OpenCV's Haar cascade classifier to detect faces.
2. **Mouth Region Analysis**: The lower half of the detected face is analyzed to detect movement.
3. **Thresholding & Pixel Count**: A binary threshold is applied to determine if a significant white region is present, indicating a drinking motion.
4. **Sound Alert**: If drinking is detected, a sound is played using Pygame.

## How to Run

1. Ensure you have a webcam connected.
2. Place a sound file (e.g., `mixkit-click-melodic-tone-1129.wav`) in the same directory as the script.
3. Run the script:

```sh
python coffee_drinking_detection.py
```

## Expected Output

- The webcam feed will open, displaying a rectangle around detected faces.
- If drinking is detected, "Drinking coffee detected!" will be printed in the console, and a sound will play.
- The detection box is drawn in pink.

## Customization

- Adjust the **threshold value** (`10000`) to fine-tune detection accuracy.
- Modify the **BGR color values** to change the rectangle color.
- Use a different **sound file** for notifications.

This project provides a basic framework for detecting coffee drinking behavior using computer vision.

