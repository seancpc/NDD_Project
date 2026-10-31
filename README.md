# NDD — Nail Disease Detection

**[English](#english) | [繁體中文](#繁體中文)**

**[Project page](https://seancpc.github.io/NDD_Project/)**

---

<a id="english"></a>

## English

Take a photo of a nail and send it to a LINE Bot: the system crops the nail region with YOLOv8 Nano, classifies the lesion with EfficientNetV2 + CBAM, and replies with a preliminary read and a recommended medical specialty. For reference only; not a medical diagnostic tool.

- **Results:** 95% average evaluation accuracy, 86% on real user smartphone photos; about 1.5 s end-to-end
- **Tech stack:** YOLOv8 Nano, EfficientNetV2 + CBAM, PyTorch (Focal Loss, Mixup / CutMix), Score-CAM, SHAP, ONNX, FastAPI + Uvicorn + Nginx, AWS EC2 / RDS (MySQL), LINE Bot (FlexMessage)

This repository hosts the project page and its figures. The full write-up, architecture and development journey are on the [project page](https://seancpc.github.io/NDD_Project/).

---

<a id="繁體中文"></a>

## 繁體中文

用手機拍下指甲照片傳給 LINE Bot,系統以 YOLOv8 Nano 自動裁切指甲區域,再以 EfficientNetV2 + CBAM 判別病變類型,回傳初步判讀與就醫科別建議。輔助參考性質,非醫療診斷工具。

- **成果**:分類評估準確率平均 95%,用戶手機實拍照片實測 86%;端到端約 1.5 秒
- **技術堆疊**:YOLOv8 Nano、EfficientNetV2 + CBAM、PyTorch(Focal Loss、Mixup / CutMix)、Score-CAM、SHAP、ONNX、FastAPI + Uvicorn + Nginx、AWS EC2 / RDS(MySQL)、LINE Bot(FlexMessage)

本 repo 存放專案頁與圖表;完整說明、系統架構與開發歷程請見[專案頁](https://seancpc.github.io/NDD_Project/)。
