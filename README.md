# 🎯 Cross-Camera-player-mapping-using-YOLO


> ⚽ Player Identity Tracking Across Multiple Camera Angles  
> 📽️ `broadcast.mp4` & `tacticam.mp4`

---

## 📌 Objective

The goal of this project is to **map and track players across two different video feeds** (`broadcast.mp4` and `tacticam.mp4`) so that each player retains a **consistent ID** in both views.

This is a classic **cross-camera multi-object tracking** problem with the added challenge of variable perspectives.

---
## 🧠 Approach

### 🎯 Object Detection
- Used the provided fine-tuned **YOLOv11** model to detect **players** and the **ball** in both videos.

### 🧬 Feature Extraction
- Extracted **visual embeddings**: color histograms, bounding box coordinates, etc.
- Applied **temporal smoothing** to ensure consistent feature tracking over time.

### 🔄 Cross-Camera Mapping
Mapped players across the two videos using:
- 📍 **Spatial Proximity**
- 🖼️ **Visual Similarity**
- ⏱️ **Temporal Consistency**

Each player was assigned a **unified `player_id`** across both feeds.

---

## 📂 Files & Structure

```bash
