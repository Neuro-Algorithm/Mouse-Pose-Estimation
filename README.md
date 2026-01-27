Mouse Pose Estimation using DeepLabCut SuperAnimal
Automated behavioral analysis pipeline for tracking mouse movement in videos using deep learning.

About The Project
This project provides a complete solution for analyzing mouse behavior in research videos. Using DeepLabCut's pre-trained SuperAnimal models, it automatically tracks 39 body keypoints across every frame of your video - without requiring any manual labeling or model training.
The entire pipeline runs in Google Colab with free GPU access, making advanced pose estimation accessible to any researcher with a web browser and mouse behavioral videos.
What It Does

Analyzes mouse videos using state-of-the-art deep learning models
Tracks 39 body landmarks including head, ears, spine, tail, and all four limbs
Generates labeled videos with keypoints and skeleton overlay
Exports tracking data in multiple formats (HDF5, CSV)
Calculates behavioral metrics like speed, distance traveled, and movement patterns


Key Features

Zero setup required - Runs entirely in Google Colab
No training needed - Pre-trained models work immediately
No GPU required locally - Uses free cloud computing
39 keypoints tracked - Complete body coverage from nose to tail
High accuracy - Built on DeepLabCut framework used in 2000+ research papers
Easy export - Get CSV files for Excel, R, MATLAB, or Python analysis


Technical Details
Models Used:

SuperAnimal Quadruped (pre-trained on 45+ species)
HRNet-W32 architecture for pose estimation
Faster R-CNN for mouse detection

Tracked Bodyparts (39 total):

Head: nose, eyes, jaw, ears (base and tips)
Body: neck, spine, tail, belly
Limbs: shoulders, knees, paws (all four legs)

Output Files:

HDF5 files with complete tracking data
CSV files for easy analysis
Labeled MP4 videos with visualizations
Trajectory plots and behavioral metrics


Quick Start

Open the Colab notebook from this repository
Upload your mouse video to Google Drive
Run the cells to analyze your video
Download labeled videos and tracking data

Processing time: ~2-5 minutes for a 30-second video

Use Cases
Perfect for researchers studying:

Locomotor activity - Open field tests, rotarod performance
Drug effects - Pharmacological impact on movement
Disease models - Parkinson's, Huntington's, stroke recovery
Genetic phenotyping - Behavioral differences in mutants
Pain assessment - Movement pattern changes
Circadian rhythms - 24-hour activity monitoring


What You Get
After processing your video, you receive:

Labeled video (.mp4) - Your original video with tracked keypoints overlaid
Tracking data (.h5, .csv) - X, Y coordinates and confidence scores for all 39 keypoints per frame
Analysis plots - Movement trajectories, speed graphs, quality metrics
Behavioral metrics - Distance traveled, average speed, activity patterns


Acknowledgments
Built using DeepLabCut framework developed by the Mathis Lab at EPFL. SuperAnimal models enable zero-shot pose estimation across species without custom training.

License
This project uses DeepLabCut (LGPL-3.0 License).

Citation
If you use this pipeline in your research, please cite:
DeepLabCut:

Mathis et al. (2018). DeepLabCut: markerless pose estimation of user-defined body parts with deep learning. Nature Neuroscience, 21(9), 1281-1289.

SuperAnimal:

Ye et al. (2024). SuperAnimal pretrained pose estimation models for behavioral analysis. Nature Communications, 15, 6529.
Communications, 15, 6529.
