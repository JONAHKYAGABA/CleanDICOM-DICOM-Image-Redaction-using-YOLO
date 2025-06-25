# 🩻 CleanDICOM: DICOM Image Redaction using YOLO

This project implements a privacy-preserving pipeline for **cleaning sensitive patient information** from **DICOM medical images** using a **YOLO object detection model** and pixel-based redaction. It supports reading `.dcm` files, detecting personally identifiable information (PII), and saving sanitized outputs.

---

## 🎯 Objectives

- ✅ Read and visualize DICOM images
- ✅ Run YOLOv8 inference to detect bounding boxes around PII (e.g., patient names)
- ✅ Redact (mask or crop) sensitive regions using bounding boxes
- ✅ Save a sanitized version of the image back into the DICOM format

---

## 🧰 Requirements

Install dependencies:

```bash
pip install pydicom numpy matplotlib pillow ultralytics
