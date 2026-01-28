[EN](README.md) | **DE**

<p align="center">
  <img src="docs/assets/Logo.png" alt="VolumanXR Logo" width="300"/>
</p>

# VolumanXR

**Eine End-to-End-Pipeline für volumetrische Erfassung und 4D-Gaussian-Darstellung**

Willkommen im zentralen Repository von **VolumanXR**, einem gemeinsamen Forschungsprojekt im Masterstudiengang Medientechnologie an der TH Köln. Ziel des Projekts ist die Entwicklung einer modularen Pipeline zur Erfassung, Verarbeitung und Visualisierung dynamischer menschlicher Darstellungen mithilfe modernster 4D-Gaussian-Splatting-Techniken — mit auf Meta Quest fokusierter XR-Integration.

## 🧠 Projektumfang

VolumanXR bietet ein skalierbares End-to-End-System mit folgenden Kernfunktionen:

- Synchronisierte Multiview-Videoaufnahme mittels eines maßgeschneiderten Volumen-Rigs
- Datenverarbeitung und Training zu dynamischen 4D-Gaussian-Repräsentationen
- Echtzeit-Visualisierung in einer immersiven XR-Umgebung
- Erweiterte Avatardarstellung durch HAC-Gaussians

## 🗂 Projektstruktur
```text
VolumanXR/ 
├── docs/                       # Dokumentation und Präsentationsmaterial 
│ ├── assets/                   # Logos und gemeinsame Ressourcen für README & Doku 
│ ├── documentation/            # Ausführliche Dokumente (PDF, LaTeX, etc.) 
│ └── PowerPoint/               # Präsentationsfolien und Visuals 
├── volumetric-capture-system/  # Multikamera-Hardware und Steuerungssoftware (Raspberry Pi) 
├── Training/                   # Preprocessing und Training mit Spacetime Gaussians 
├── Viewer/                     # WebXR/WebGPU-Viewer zur volumetrischen Echtzeitvisualisierung 
├── [hac-gaussian/]             # ⚠️ Wird in einem separaten ZIP-Archiv zur Verfügung gestellt
├── LICENSE 
└── README.md                   # Du bist hier :)
```

Jedes Hauptverzeichnis entspricht einem Teilprojekt. Für Setup-Anleitungen und technische Details siehe die `README.md`-Dateien in den jeweiligen Unterordnern.

## 🔍 Teilprojekte im Überblick

### [**Volumetric Capture System**](volumetric-capture-system/) 
Konstruktion und Steuerung des Kamera-Rigs (68 Raspberry Pis + Kameras):

- WLAN-Synchronisation und Fernsteuerung
- GUI zur zentralen Aufnahmeverwaltung
- Automatisierte Kalibrierung und Session-Management

### [**Training Pipeline**](training/) 
Pipeline zur Verarbeitung und zum Training von 4D Spacetime Gaussians:

- COLMAP-basierte Kameratracking-Verfahren
- Hintergrundentfernung und Feature-Filterung
- Trainingsprozesse & Szeneoptimierung
- Synthetische Datensätze für Testzwecke

### [**Viewer**](web-viewer/) 
Ein selbst entwickelter WebXR/WebGPU-Viewer zur immersiven Wiedergabe von gaußbasiert gerenderten volumetrischen Inhalten in XR:

- Kompatibel mit Meta Quest VR-Brillen
- Interaktive Steuerung (Platzierung, Skalierung, Rotation)
- Sequenzübergänge und Glättung

### **HAC-Gaussian**
Experimentelle Arbeiten mit animierbaren Avataren auf Basis von 3D-Gaussian-Splatting:

- Nutzung von Animatable Gaussians
- Mixed Precision Training
- Optimierung für Echtzeitanwendungen

## 📄 Dokumentation

Die vollständige Projektdokumentation befindet sich unter `docs/documentation/`  
Präsentationsmaterial und Folien unter `docs/PowerPoint/`  
Projektweite Logos und Grafiken befinden sich in `docs/assets/`.

## 👥 Projektteam

Dieses Projekt wurde von folgenden Teammitgliedern umgesetzt:

- Kai Altwicker (stellv. Projektleitung)
- Dennis Luca Amuser
- Matthias Bullert
- David Martin Karg
- David Mertens
- Alisa Rüge
- Steffen Stein (Projektleitung)
- Marvin Winkler

Besonderer Dank gilt dem Makerspace der TH Köln, Prof. Dr.-Ing. Arnulph Fuhrmann und der Förderung durch Kickstart@TH Köln.

## 📜 Lizenz

Dieses Projekt steht unter der MIT-Lizenz. Details siehe `LICENSE`.

---

> Für Anleitungen und spezifische Hinweise besuche bitte die READMEs in den jeweiligen Unterverzeichnissen.
