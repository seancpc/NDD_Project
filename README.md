# BP — Storefront-Sign Recognition & Payment Recommendation

**[English](#english) | [繁體中文](#繁體中文)**

**[Project page](https://seancpc.github.io/BP_Project/)**

---

<a id="english"></a>

## English

Photograph a storefront sign and send it to a LINE Bot: a ViT model classifies the store type, and the system replies with the top-3 highest-cashback payment methods for that category. No extra app required.

- **Results:** ViT accuracy 90%, raised to 97% after multi-angle and occlusion data reinforcement; inference within about 1 s
- **Dataset:** 15 store-sign classes photographed on site in Taipei's Ximending district
- **Tech stack:** ViT (compared with ResNet50 / InceptionV3 / MobileNetV2), PyTorch, Flask + Nginx (HTTPS), MySQL Views, AWS EC2 / RDS (first built on GCP, then migrated to AWS), LINE Bot (FlexMessage carousel)

This repository hosts the project page and its figures. The full write-up, architecture and development journey are on the [project page](https://seancpc.github.io/BP_Project/).

---

<a id="繁體中文"></a>

## 繁體中文

拍下商家招牌傳給 LINE Bot,ViT 模型分類店家類型,系統回傳該類店家回饋最高的前 3 名支付方式。不需安裝額外 App。

- **成果**:ViT 準確率 90%,經多角度與遮蔽物資料強化後達 97%;推論約 1 秒內
- **資料集**:台北西門町實地蒐集 15 類商家招牌
- **技術堆疊**:ViT(選型比較 ResNet50 / InceptionV3 / MobileNetV2)、PyTorch、Flask + Nginx(HTTPS)、MySQL View、AWS EC2 / RDS(初版建於 GCP,後遷移至 AWS)、LINE Bot(FlexMessage 輪播)

本 repo 存放專案頁與圖表;完整說明、系統架構與開發歷程請見[專案頁](https://seancpc.github.io/BP_Project/)。
