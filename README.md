# 📄 Hand Text Detection & Recognition Using OpenCV and OCR

**Project by:** Syeda Umaima Tamkeen

---

## 📝 Summary

This project demonstrates a **computer vision pipeline** for detecting and recognizing handwritten or printed text from images containing **hand and text regions**. Using a combination of **OpenCV for image preprocessing** and **Optical Character Recognition (OCR)** through Tesseract, the system extracts readable text from complex backgrounds such as hand-held notes.

The goal is to build a lightweight, accurate, and modular solution for text extraction in real-world scenarios, especially where documents are partially occluded or held in hands.

---

## 🔍 Key Steps

### 1. Image Acquisition & Preprocessing
- Loaded input image and resized for consistency.
- Converted to grayscale for simplification.
- Applied Gaussian blur to reduce noise.

### 2. Edge Detection & Thresholding
- Performed edge detection using Canny.
- Applied adaptive or Otsu thresholding to enhance text regions.

### 3. Contour Detection
- Used OpenCV's `findContours()` to locate hand and text blocks.
- Filtered out small/noisy contours to isolate regions of interest (ROIs).

### 4. ROI Extraction
- Extracted bounding boxes around detected text-containing regions.
- Cropped these regions for OCR.

### 5. Optical Character Recognition (OCR)
- Used **Tesseract OCR** to recognize and extract text from the cropped images.
- Post-processed OCR output to remove garbage characters and improve readability.

### 6. Visualization
- Drew bounding boxes around detected text areas.
- Displayed extracted text alongside processed images using Matplotlib or OpenCV.

---

## ✅ Results

- Successfully detected hand-held text regions from noisy and complex images.
- Extracted readable text using OCR even with partial obstructions.
- Demonstrated robustness on diverse images including printed notes, handwritten text, and natural lighting conditions.

---

## 📌 Conclusion

This project highlights the effective use of **OpenCV + Tesseract OCR** for real-world **text extraction** applications. It is particularly useful in domains like:
- Mobile document scanning
- Smart note transcription
- Assistive technologies for visually impaired users


