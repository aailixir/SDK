# 🚀 Ailixir API SDK

**AI Model & Dataset Management API for Edge AI Systems**

Ailixir API SDK provides RESTful APIs to manage AI datasets, YOLO training configurations, and release model versions in an Edge AI deployment environment.

It is designed for enterprise AI platforms, on-premise deployment, and GPU edge devices.

---

## 📌 Features

- 📂 Retrieve all AI dataset groups  
- 🤖 Manage AI model configurations  
- 🔄 Get active release model version  
- 🧠 Supports YOLOv5 / YOLOv7  
- 🏗 Designed for Edge AI architecture  
- ⚡ Lightweight local API service  

---

# 📡 API Endpoints

---

## 1️⃣ Get All AI Datasets

Retrieve all dataset groups and their associated AI models.

### Request

GET /api.php?model=all


### Sample Response

```json
[
  {
    "group_id": 1,
    "group": "Smart Healthcare",
    "ai_model": [
      {
        "ai_id": 1,
        "ai_name": "Breast Cancer Detection",
        "ai_path": "/dataset/dataset_6/",
        "local_path": "D:/Business/dataset/Breast Cancer Dataset_BUSI_with_GT",
        "ai_engine": "YOLOv5",
        "epochs": 10
      },
      {
        "ai_id": 8,
        "ai_name": "Segmentation",
        "ai_path": "/dataset/dataset_2/",
        "local_path": "C:/Program Files/Ailixir/Apache24/htdocs/dataset/dataset_2/",
        "ai_engine": "YOLOv5",
        "epochs": 10
      }
    ]
  },
  {
    "group_id": 2,
    "group": "Office Automation",
    "ai_model": [
      {
        "ai_id": 4,
        "ai_name": "Water Bottle Recognition",
        "ai_path": "/dataset/dataset_5/",
        "local_path": "D:/Business/dataset/garbage",
        "ai_engine": "YOLOv5",
        "epochs": 25
      }
    ]
  },
  {
    "group_id": 3,
    "group": "Smart Transportation",
    "ai_model": [
      {
        "ai_id": 5,
        "ai_name": "Wind Turbine Recognition",
        "ai_path": "/dataset/dataset_1/",
        "local_path": "D:/Business/dataset/traffic",
        "ai_engine": "YOLOv5",
        "epochs": 10
      },
      {
        "ai_id": 6,
        "ai_name": "Smart Vessel",
        "ai_path": "/dataset/dataset_7/",
        "local_path": "/assets/images/gallery/exp153/",
        "ai_engine": "YOLOv7",
        "epochs": 10
      },
      {
        "ai_id": 7,
        "ai_name": "Smoke and Fire Detection",
        "ai_path": "/dataset/dataset_3/",
        "local_path": "D:/Business/dataset/crack",
        "ai_engine": "YOLOv5",
        "epochs": 10
      }
    ]
  },
  {
    "group_id": 9999,
    "group": "Trash Bin",
    "ai_model": []
  }
]
```
###
Get AI release mode
###
Response
{"status":"success","msg":"Model version #2 data loaded successfully.","data":[{"id":5,"modelID":"6","yoloVersion":"YOLOv7","batchSize":8,"epochs":50,"outPath":"\/engine\/YOLOv7\/runs\/train\/temp1","datYAMLPath":"\/dataset\/dataset_7\/data.yaml","datetime":"2026-02-27 14:20:24","pid":"34592"}]}


