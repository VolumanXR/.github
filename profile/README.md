**EN** | [DE](README.de.md)

<p align="center">
  <img src="docs/assets/Logo.png" alt="VolumanXR Logo" width="300"/>
</p>

# VolumanXR

**An End-to-End Pipeline for Volumetric Capture and 4D Gaussian Rendering**

Welcome to the central repository for **VolumanXR**, a collaborative research project developed at TH Köln as part of the Medientechnology Master's program. This project provides a modular pipeline for capturing, training, and rendering high-quality, dynamic human representations using state-of-the-art 4D Gaussian Splatting techniques — with XR integration focused on Meta Quest devices.

## 🧠 Project Scope

VolumanXR delivers a scalable and reproducible end-to-end system capable of:

- Capturing synchronized multi-view video data using a custom volumetric rig
- Processing and training that data into dynamic 4D Gaussian representations
- Rendering immersive real-time visualizations within an XR environment
- Experimenting with advanced avatar deformation via HAC-Gaussians

## 🗂 Repository Structure
```text
VolumanXR/
├── docs/                       # Project documentation and presentation assets
│   ├── assets/                 # Logos and shared resources for docs and README
│   ├── documentation/          # In-depth written documentation (PDF, LaTeX, etc.)
│   └── PowerPoint/             # Presentation slides and visuals
├── volumetric-capture-system/  # Multicamera rig hardware & software (Raspberry Pi-based)
├── Training/                   # Preprocessing and Spacetime Gaussian training pipeline
├── Viewer/                     # WebXR/WebGPU-based viewer for real-time XR 
├── LICENSE
└── README.md                   # You are here :)
```

Each major directory corresponds to a subteam's work. For technical deep dives, setup instructions, and usage notes, please refer to the individual `README.md` files in those subfolders.

## 🔍 Subproject Overview

### [**Volumetric Capture System**](volumetric-capture-system/) 
Hardware construction and software orchestration of the capture rig (68 Raspberry Pis + Cameras), including:

- Synchronization and remote control over WiFi
- Capture controller with GUI
- Automated calibration and session management

### [**Training Pipeline**](training/) 
A data processing and training pipeline for 4D Spacetime Gaussians, including:

- COLMAP-based camera tracking
- Background and feature stripping
- Scene optimization and training
- Synthetic dataset generation for testing

### [**Viewer**](web-viewer/) 
A custom WebXR/WebGPU viewer for immersive playback of Gaussian-rendered volumetric content in XR:

- Compatible with Meta Quest devices
- Interactive placement, scaling, and playback control
- Sequence stitching and transition smoothing

### **HAC-Gaussian**
Experimental work on Humanoid Animated Characters using 3D Gaussian splats with techniques such as:

- Animatable Gaussians
- Mixed-precision training
- Real-time rendering optimizations

## 📄 Documentation

A full project report is available under `docs/documentation/`  
Slides and visual assets used for presentations can be found in `docs/PowerPoint/`.  
Teamwide branding and visual assets (e.g. logo) are stored in `docs/assets/`.

## 👥 Contributors

This project was developed by the following team members:

- [Kai Altwicker](https://github.com/tallAldi) (Project Co-Lead)
- [Dennis Luca Amuser](https://github.com/dooonnis)
- [Matthias Bullert](https://github.com/DuesenDan)
- [David Martin Karg](https://github.com/EmptyBarrel)
- [David Mertens](https://github.com/DavidMertTH)
- [Alisa Rüge](https://github.com/validP0)
- [Steffen Stein](https://github.com/forEachWhileTrue) (Project Lead)
- [Marvin Winkler](https://github.com/Knobelboy)

Special thanks to the TH Köln Makerspace, Prof. Dr.-Ing. Arnulph Fuhrmann, and the Kickstart@TH Köln initiative for their generous support.

## 📜 License

This project is licensed under the MIT License. See `LICENSE` for details.

---

> For detailed setup or usage instructions, check the README inside each subdirectory.


        
