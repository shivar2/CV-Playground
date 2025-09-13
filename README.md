# CV-Playground
A compact OpenCV practice project showing fundamental image processing techniques:

- Spatial filtering (Gaussian blur, etc.)
- Geometric transforms (rotation, perspective)
- Edge and corner detection (Canny, Harris)
- Feature detection and matching (SIFT, ORB)

# Requirements
- Python 3.x
- OpenCV (cv2)
    - Optional: opencv-contrib-python for SIFT
 
```
pip install opencv-python
# or for full feature modules
pip install opencv-contrib-python
```

# Highlights
- Gaussian blur before edge detection to reduce noise and improve robustness of subsequent operations.
- Histogram analysis:
    - Intensity histograms and normalized cumulative histograms to understand image brightness distribution.
    - Histogram equalization and optional CLAHE (Contrast Limited Adaptive Histogram Equalization) to enhance contrast.
    - Quantitative insights: mean/median intensity, standard deviation, histogram-based similarity metrics (e.g., histogram intersection, correlation) before/after processing.
- Geometric transforms:
    - Rotation: demonstrate how to rotate images around a center with cv.getRotationMatrix2D and cv.warpAffine.
    - Perspective: simulate view changes with cv.getPerspectiveTransform / cv.warpPerspective.
- Edge and corner detection:
    - Canny edge detector with tunable thresholds for different lighting/narratives.
    - Harris corner detector to identify salient points.
- Feature detection and matching:
    - SIFT and ORB descriptors with a simple matcher (BFMatcher) and ratio-test considerations.
    - Demonstrates robustness under geometric changes and lighting variations.

