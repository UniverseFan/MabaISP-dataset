# MambaISP-Dataset (Official Repository)

This is the official repository for the dataset and data pipelines introduced in **"MambaISP: Advanced Low-Light Image Enhancement via State Space Models"**. 

This project features an independently constructed, high-quality low-light image enhancement corpus and a complete full-link physical noise simulation model, designed to bridge the gap between ideal laboratory training and real-world complex imaging degradation.

---

## 📢 Dataset Download

Due to GitHub's file size limitations, the full high-quality dataset is hosted on **Baidu Network Disk (百度网盘)**. 

- **Download Link:** [Baidu Wangpan Link](https://pan.baidu.com/s/1BFfEP-yJsfRKF7-W43NH1w?pwd=mtky) 
- **Extraction Code (提取码):** `mtky`

---

## 🌟 Key Features

1. **High-Quality Low-Light Corpus:** Unlike traditional synthetically degraded images, our corpus captures/models authentic structural and semantic details under low-illumination constraints, providing a challenging benchmark for computer vision backends.
2. **Full-Link Physical Noise Model:** We provide the integrated pipeline scripts to simulate real sensor noise profiles (e.g., photon shot noise, read noise) based on real physical imaging baselines, which significantly improves the model's out-of-distribution generalization.
3. **Hardware-Friendly Alignments:** Fully compatible with edge AI platforms (such as AX650N) for real-time video and image signal processing (ISP) application deployment.

---

## 📂 Dataset Structure

After downloading and extracting the dataset from the Baidu Wangpan link, please arrange the directories as follows to match our evaluation and training protocols:

```text
./MambaISP-dataset/
  ├── train/
  │   ├── low/          # Input low-light images (with real/simulated physical noise)
  │   └── high/         # Ground truth high-quality reference images
  ├── val/
  │   ├── low/          
  │   └── high/         
  └── scripts/
      └── noise_model.py # Full-link physical noise generation script
