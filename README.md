# FLP Renamer AI

> **Intelligent FL Studio Project Mixer Track Organization**
> ## ⬇️ Download Release
> Download the _**[FLP Renamer AI v1.0 installer](https://github.com/chemozione/FLP-Renamer-AI/releases/download/v1.0.0/FLP_Renamer_AI_1.0.0_Setup.exe)**_ from GitHub
> 
> ![Alt text](/Screenshot.png?raw=true "Renamed FLP Screenshot in FL Studio")

A powerful AI-driven tool that automatically categorizes and renames mixer tracks in FL Studio project files (.flp). Built with machine learning models trained on thousands of track names, it intelligently suggests meaningful prefixes and color coding for better project organization.

## 🚀 Features

- **AI-Powered Classification**: Advanced machine learning models with 92%+ accuracy
- **40+ Track Categories**: Comprehensive support for all music production elements
- **Smart Color Coding**: Automatic color assignment based on track categories
- **Batch Processing**: Handle multiple projects efficiently
- **Backup & Safety**: Built-in backup creation and dry-run modes
- **Real-time Preview**: See changes before applying them

![Alt text](/Screenshot_2.png?raw=true "FLP Renamer AI GUI")

## 🎯 Supported Track Categories

### Core Instrument Categories
| Category | Description | Examples |
|----------|-------------|----------|
| **DRUMS_** | Percussion elements | Kick, snare, hi-hat, crash, toms |
| **BASS_** | Low-frequency instruments | Bass lines, sub-bass, 808, bass synth |
| **GUIT_** | String instruments | Guitar, acoustic, electric, distorted |
| **KEYS_** | Keyboard instruments | Piano, keyboard, rhodes, organ |
| **SYNTH_** | Synthesized sounds | Lead, pad, arp, pluck, bass |
| **VOX_** | Vocal elements | Lead vocal, backing vocal, harmony |
| **INST_** | Orchestral instruments | Strings, brass, woodwind, orchestral |

### Specialized Categories
| Category | Description | Examples |
|----------|-------------|----------|
| **AMBI_** | Atmospheric elements | Ambient, atmosphere, pad, drone |
| **FX_** | Effects and processing | Reverb, delay, chorus, distortion |
| **BUS_** | Routing and mixing | Bus, aux, send, return, submix |
| **MASTER_** | Final processing | Master, print, bounce, final |
| **SAMP_** | Sample-based content | Sample, loop, one-shot, stinger |

## 📊 AI Model Performance

Our machine learning models achieve exceptional accuracy:

| Model | Accuracy | F1-Score | Cross-Validation |
|-------|----------|----------|------------------|
| **Random Forest** | 92.5% | 92.0% | 91.8% |
| **Gradient Boosting** | 91.5% | 91.0% | 91.5% |
| **Logistic Regression** | 90.8% | 90.2% | 90.8% |

**Production Model**: Random Forest with 92.5% test accuracy

## 🛠️ Installation & Setup

### Prerequisites
- Windows 10/11
- FL Studio (for .flp file compatibility)
- Python 3.8+ (for AI model components)

### Quick Start

> **⚠️ Important**: This repository uses Git LFS for large executable files. Downloading as ZIP from GitHub will give you corrupted files. See [Download Instructions](DOWNLOAD_INSTRUCTIONS.md) for proper setup.

#### Option 1: Clone with Git LFS (Recommended)
```bash
git clone https://github.com/chemozione/FLP-Renamer-AI.git
cd FLP-Renamer-AI
git lfs pull
```

#### Option 2: Download from Releases
1. Go to the [Releases](https://github.com/chemozione/FLP-Renamer-AI/releases) page
2. Download the latest release package
3. Extract and run `FLPRenamerUI.exe`

## 📖 User Guide

### Getting Started

1. **Configure Core Path**
   - Point "Core EXE" to `FLPRenamerCore.exe`
   - This handles the AI processing and FLP file manipulation

2. **Load Your Project**
   - Click "Browse" to select your .flp file
   - Output path is auto-suggested (you can override if needed)

3. **Configure Options**
   - **Force Colors**: Apply category-based color coding to mixer tracks
   - **Create Backup**: Automatically backup original files before changes
   - **Dry Run**: Preview changes without modifying files
   - **Verbose**: Enable detailed logging for troubleshooting
   - **Custom Prefixes**: Modify the category prefix list

### Color Coding Setup

For optimal color coding functionality:

1. Open your .flp file in FL Studio
2. Navigate to mixer tracks (F9)
3. Select all tracks (Ctrl+A)
4. Change track colors (double-click F2) and confirm
5. Save the project
6. Now "Force Colors" will work as expected

### Workflow Actions

| Action | Description |
|--------|-------------|
| **Preview** | Analyze tracks and show suggested names |
| **Apply** | Apply changes and save new FLP file |
| **Sort Guide** | Generate text-based organization guide |
| **Analyze** | Run detailed project analysis |

### Interface Tabs

- **Summary**: Category counts and processing output
- **Sort Guide**: Text instructions for manual organization
- **Analysis**: Detailed project analysis reports
- **Logs**: System output and error information

## 🔧 Technical Details

### AI Model Architecture
- **Feature Engineering**: Advanced text preprocessing and feature extraction
- **Data Augmentation**: Enhanced training with synthetic data
- **Ensemble Methods**: Multiple model voting for improved accuracy
- **Cross-Validation**: Robust performance evaluation

### File Structure
```
FLP-Renamer-AI/
├── ai_model/                 # AI model components
│   ├── mixer_classifier_model.joblib
│   ├── mixer_track_classifier.py
│   └── predict_track_names.py
├── FLPRenamerUI.exe         # Main application
├── FLPRenamerCore.exe       # AI processing engine
└── color_palette.json       # Color scheme definitions
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

- **Issues**: Report bugs and request features on [GitHub Issues](https://github.com/chemozione/FLP-Renamer-AI/issues)
- **Discussions**: Join the community on [GitHub Discussions](https://github.com/chemozione/FLP-Renamer-AI/discussions)

## 🙏 Acknowledgments

- **[PyFLP](https://github.com/demberto/PyFLP)** - Essential reference for FL Studio project file reverse engineering and parsing
- **FL Studio community** for inspiration and feedback
- **Open source machine learning libraries** for AI model development
- **Contributors and testers** who helped improve the tool

---

**Made with ❤️ for the FL Studio community**
