# SMPL Blender Add-on for Blender 4.5+

![Blender Version](https://img.shields.io/badge/Blender-4.5+-orange)
![License](https://img.shields.io/badge/License-GPL%20v2-blue)
![SMPL](https://img.shields.io/badge/SMPL-Compatible-green)

## 🌟 **Updated for Blender 4.5 Compatibility**

This is an **updated version** of the original SMPL Blender add-on that has been **specifically modified to work with Blender 4.5 and newer versions**. The original add-on had compatibility issues with newer Blender versions, which have been resolved in this fork.

## 📖 About

This add-on allows you to add gender-specific [SMPL](https://smpl.is.tue.mpg.de) (Skinned Multi-Person Linear) model skinned meshes to your Blender scene. Each imported SMPL mesh consists of a shape-specific rig, as well as shape keys (blend shapes) for shape, expression and pose correctives.

SMPL is a realistic 3D model of the human body that can be used for computer vision, graphics, and machine learning applications.

## ✨ Features

- ✅ **Add gender-specific SMPL mesh** to current scene (Male/Female)
- 🎨 **Set mesh textures** (None, UV Grid, Color Grid)
- 📏 **Position feet on ground plane** (z=0)
- 🎲 **Randomize/reset body shape**
- 🦴 **Update joint locations**
- 🔧 **Enable/disable corrective pose shapes**
- 📝 **Export current pose** in SMPL theta notation to console
- 📦 **FBX export to Unity** with multiple options:
  - Import without rotations and scaling issues
  - Shape key export options:
    - Body shape + pose correctives
    - Body shape only  
    - None (bakes current shape into mesh)

## 🎯 Requirements

- **Blender 4.5+** (Updated compatibility)
- **No additional dependencies** required

## 💾 Installation

1. **Download** the latest release from this repository
2. Open **Blender** → **Edit** → **Preferences** → **Add-ons**
3. Click **Install** and select the downloaded ZIP file
4. **Enable** the "SMPL for Blender" add-on
5. In the 3D Viewport, enable the **Sidebar** via **View** → **Sidebar** (or press `N`)
6. The **SMPL tool panel** will appear in the sidebar

## 🎬 Usage Tutorial

For a comprehensive usage tutorial, please refer to this YouTube video:
**[SMPLX for Blender Tutorial](https://www.youtube.com/watch?v=m8i00zG6mZI&t=336s)**

> **Note:** While this tutorial is for SMPLX, the plugin usage methods are very similar to this SMPL add-on. The interface and workflow are nearly identical.

## 🔧 What's Fixed

This version resolves compatibility issues with Blender 4.5+ that were present in the original add-on, specifically:
- Updated API calls for Blender 4.5+
- Fixed deprecated function usage
- Ensured proper panel registration
- Resolved UI layout issues

## 📁 Project Structure

```
smpl_blender_addon/
├── __init__.py                          # Main add-on file (updated for Blender 4.5+)
├── LICENSE.md                           # License information
├── README.md                           # This file
└── data/
    ├── smpl-model-20200803.blend       # SMPL model data
    ├── smpl_joint_regressor_female.npz # Female joint regressor
    └── smpl_joint_regressor_male.npz   # Male joint regressor
```

## 📄 License

- **Generated body mesh data** using this add-on:
  - Licensed under [SMPL Model License](https://smpl.is.tue.mpg.de/modellicense)
- See `LICENSE.md` for complete license information including commercial licensing
- **Attribution for publications**: You agree to cite the most recent paper describing the model as specified on the [SMPL website](https://smpl.is.tue.mpg.de)

## 🤝 Contributing

Issues and pull requests are welcome! If you encounter any problems with Blender 4.5+ compatibility, please open an issue.

## 📚 References

- [Original SMPL website](https://smpl.is.tue.mpg.de)
- [SMPL paper and citations](https://smpl.is.tue.mpg.de)
- [Usage tutorial (SMPLX)](https://www.youtube.com/watch?v=m8i00zG6mZI&t=336s)

## ⭐ Credits

- **Original Author**: Joachim Tesch, Max Planck Institute for Intelligent Systems
- **Blender 4.5+ Compatibility**: Updated by [lu123bing](https://github.com/lu123bing)

---

If you find this add-on useful, please consider giving it a ⭐ on GitHub!
