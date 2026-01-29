**EN** | [DE](README.de.md)

<p align="center">
  <img src="../docs/assets/Logo.png" alt="VolumanXR Logo" width="300"/>
</p>

# VolumanXR

**An End-to-End Pipeline for Volumetric Capture and 4D Gaussian Rendering**

Welcome to the **VolumanXR GitHub organization**, which hosts the repositories of a collaborative research project developed at TH Köln as part of the Medientechnology Master’s program. VolumanXR provides a modular ecosystem for capturing, training, and rendering high-quality, dynamic human representations using state-of-the-art 4D Gaussian Splatting techniques, with XR integration focused on Meta Quest devices.

Each subteam maintains its own repository within this organization, together forming a complete end-to-end pipeline.
> **Maintenance Notice**\
>This GitHub organization primarily serves as a documentation and reference space for the VolumanXR research project. Further development occurs on an occasional basis and is not continuous. Repositories may receive updates from time to time, but regular maintenance and long-term support should not be assumed.

## 🧠 Project Scope

VolumanXR delivers a scalable and reproducible end-to-end system capable of:

- Capturing synchronized multi-view video data using a custom volumetric rig
- Processing and training that data into dynamic 4D Gaussian representations
- Rendering immersive real-time visualizations within an XR environment
- Experimenting with advanced avatar deformation via HAC-Gaussians

## 🗂 Organization Structure
The VolumanXR organization is composed of multiple repositories, each owned by a dedicated subteam. For now only the capture system is public:
```text
VolumanXR (GitHub Organization)
├── docs/                       # Shared project documentation and assets
│   ├── assets/                 # Logos and shared resources for docs and README
│   └── publications/           # Documentation and publications
├── volumetric-capture-system/  # Multicamera rig hardware & software (Raspberry Pi-based)
├── training/                   # Preprocessing and spacetime Gaussian training pipeline
├── viewer/                     # WebXR/WebGPU-based viewer for real-time XR
├── hac-gaussian/               # Experimental animatable Gaussian avatar research
└── .github/README.md           # Organization README                               <-- You are here :)
```

Each repository contains its own `README.md` with technical details, setup instructions, and usage documentation specific to that subproject.

## 🔍 Subproject Overview

### [**Volumetric Capture System**](https://github.com/VolumanXR/volumetric-capture-system) (public repository)
Hardware construction and software orchestration of the capture rig (68 Raspberry Pis + Cameras), including:

- Synchronization and remote control over WiFi
- Capture controller with GUI
- Automated calibration and session management

### **Training Pipeline** (internal only)
A data processing and training pipeline for 4D Spacetime Gaussians, including:

- COLMAP-based camera tracking
- Background and feature stripping
- Scene optimization and training
- Synthetic dataset generation for testing

### **Viewer** (internal only)
A custom WebXR/WebGPU viewer for immersive playback of Gaussian-rendered volumetric content in XR:

- Compatible with Meta Quest devices
- Interactive placement, scaling, and playback control
- Sequence stitching and transition smoothing

### **HAC-Gaussian** (internal only)
Experimental work on Humanoid Animated Characters using 3D Gaussian splats with techniques such as:

- Animatable Gaussians
- Mixed-precision training
- Real-time rendering optimizations

## 📄 Documentation

A full project report is available under [`docs/publications/Voluman_Documentation_DE.pdf`](../docs/publications/Voluman_Documentation_DE.pdf)  (German only)

Parts of this project have been published as an [IEEE VR26 Poster](../docs/publications/IEEE_VR26_Poster.pdf), covering the Volumetric Capture System, see the corresponding repository for details.

Teamwide branding and visual assets (e.g. logo) are stored in `docs/assets/`.

## 👥 Contributors

This project was developed by the following team members:

#### Volumetric Capture System

- [Kai Altwicker](https://github.com/tallAldi) (Project Co-Lead)
- [Dennis Luca Amuser](https://github.com/dooonnis)

#### Training Pipeline
- [Matthias Bullert](https://github.com/DuesenDan)
- [David Mertens](https://github.com/DavidMertTH)

#### Viewer
- [David Martin Karg](https://github.com/EmptyBarrel)
- [Alisa Rüge](https://github.com/validP0)
- [Steffen Stein](https://github.com/forEachWhileTrue) (Project Lead)

#### HAC-Gaussian
- [Marvin Winkler](https://github.com/Knobelboy)

Special thanks to the TH Köln Makerspace, Prof. Dr.-Ing. Arnulph Fuhrmann, and the Kickstart@TH Köln initiative for their generous support.

## 📜 License

This project is licensed under the MIT License. See `LICENSE` for details.

---

> For detailed setup or usage instructions, check the README inside each subdirectory.


        
