# Shop Lifting Detection System

## Overview

This project implements an advanced computer vision-based shop lifting detection system. By leveraging state-of-the-art AI models, specifically SAM2 (Segment Anything Model 2) and Florence 2, along with sophisticated image processing techniques, our system analyzes video feeds from store cameras in real-time to identify suspicious behavior and potential shop lifting incidents.

## Key Features

- **Real-time Video Processing**: Efficiently processes video streams from multiple store cameras.
- **Advanced Object Detection**: Utilizes SAM2 for precise object segmentation and Florence 2 for robust object recognition and scene understanding.
- **Behavior Analysis**: Employs sophisticated machine learning algorithms to analyze customer behavior and movement patterns.
- **Alert System**: Generates real-time alerts for store personnel when suspicious activity is detected.
- **Privacy-Preserving**: Implements face pixelation to protect customer privacy in stored footage.

## Technical Stack

- **AI Models**: 
  - SAM2 (Segment Anything Model 2) for precise object segmentation
  - Florence 2 for advanced object recognition and visual understanding
- **Face Detection**: Cutting-edge algorithms for identifying and tracking individuals in frame
- **Video Processing**: OpenCV for efficient frame extraction and video compilation
- **Pixelation**: Custom algorithm to obscure faces in stored footage
- **Deep Learning Framework**: PyTorch

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/JerripotulaSriharsha/shop_lifting_detection-.git
   cd shop-lifting-detection
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Download the required model weights:
   ```
   python download_models.py
   ```

## Usage

1. To process a single video file:
   ```
   python detect_shoplifting.py --input path/to/video.mp4 --output path/to/output.mp4
   ```

2. To start real-time detection on a camera feed:
   ```
   python realtime_detection.py --camera_id 0
   ```

## Configuration

Adjust detection sensitivity and other parameters in `config.yaml`. You can fine-tune the behavior of SAM2 and Florence 2 models separately for optimal performance in your specific store environment.

## Contributing

We welcome contributions to improve the shop lifting detection system. Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgments

- SAM2 model by Meta AI Research
- Florence 2 model by Microsoft Research
- OpenCV community for video processing tools

## Technical Details

### SAM2 (Segment Anything Model 2)
SAM2 is used for its exceptional ability to perform precise object segmentation. In our system, it helps in accurately isolating individual objects and people in the video feed, which is crucial for detecting potential shop lifting activities.

### Florence 2
Florence 2 is a versatile vision model that we employ for its advanced object recognition and scene understanding capabilities. It complements SAM2 by providing high-level interpretation of the segmented objects and their interactions within the store environment.

### Integration
Our system integrates the outputs of SAM2 and Florence 2 to create a comprehensive understanding of the store scene. This integration allows for more accurate detection of suspicious behaviors associated with shop lifting.

## Disclaimer

This system is designed to assist in the detection of potential shop lifting incidents. It should be used in conjunction with trained security personnel and established store policies. The developers are not responsible for any misuse or legal implications arising from the use of this system.
