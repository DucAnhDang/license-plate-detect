# 📸 License Plate Recognition (LPR) with Manual Cropping and OCR

## 🔎 Overview
This project focuses on recognizing vehicle license plates from **manually cropped images** using **OCR (Optical Character Recognition)**. The system is designed for Vietnamese license plates but can be adapted to other countries.

Currently, license plates are cropped manually from input images, and then the cropped plate images are passed through the OCR module for text recognition.

## ✅ Features
- Manual license plate cropping
- OCR recognition using **EasyOCR / PaddleOCR**
- Supports image inputs
- Post-processing with regex to filter valid Vietnamese license plate formats
- Export results as text files

## 🗂 Dataset
- Images of cropped license plates collected manually
- Contains various license plate styles, fonts, and lighting conditions
- Example dataset source: Vietnamese streets

## ⚙️ Technology Stack
| Tool | Description |
|-----|------------|
| **Python** | Programming Language |
| **EasyOCR / PaddleOCR** | OCR engine for text extraction |
| **OpenCV** | Image processing |

## 🚀 Installation
```bash
git clone https://github.com/DucAnhDang/license-plate-detect.git
cd license-plate-detect
pip install -r requirements.txt
```

## 🛠 Usage
Place your **manually cropped license plate images** in the `cropped_plates/`.

### Run OCR on all images:
```bash
python src/ocr.py --input_dir cropped_plates/
```

### Example Output:
```
plate1.jpg -> Recognized Plate: 19-X1 159.8
plate2.jpg -> Recognized Plate: 29-AA 123.45
```

## 📈 Sample Result
| Image | OCR Result |
|------|-----------|
| ![Example Plate](results/sample_plate.jpg) | 19-X1 159.8 |

## 💡 Future Improvements
- Integrate automatic license plate detection using YOLOv8
- Real-time video processing
- Export results to a database or web interface

## 🙌 Credits
- [EasyOCR](https://github.com/JaidedAI/EasyOCR)
- [OpenCV](https://opencv.org/)

## 📃 License
This project is licensed under the MIT License - see the LICENSE file for details.
