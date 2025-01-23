# Differentiable Mobile Display Photometric Stereo (DMDPS)

![DMDPS Visualization](https://github.com/user-attachments/assets/5ef9f598-1635-4875-b33c-7ee7813a8f59)

## Overview

Display photometric stereo reconstructs surface normals under diverse illumination patterns using a monitor. Recently, **Differentiable Display Photometric Stereo (DDPS)** demonstrated improved surface normal reconstruction accuracy by learning display patterns. However, previous methods faced several limitations, such as:
- Requiring a completely dark room
- Needing a fixed shooting setup
- Dependency on specialized equipment like polarization cameras and LCD monitors

To address these issues, we propose **Differentiable Mobile Display Photometric Stereo (DMDPS)**, which extends DDPS by leveraging mobile devices and high-dynamic-range (HDR) imaging. This approach enables flexible shooting locations and eliminates the need for a dark room.

---

## Key Contributions

1. **Mobile Device Integration**:
   - Developed a mobile app for simultaneous pattern display and image capture.
   - Tested with devices like the Samsung Galaxy S22 for high-quality results.

2. **Learning Display Patterns**:
   - DMDPS learns optimal display patterns via the app.
   - Trains on real-world 3D-printed objects with corresponding base patterns for supervision.

3. **Improved Reconstruction Accuracy**:
   - Error using unlearned patterns: **0.07394**
   - Error using learned patterns: **0.05337**

4. **Database Creation**:
   - Built a database of reconstructed surface normals and albedos for wild objects (e.g., fall leaves).
   - Data is publicly disclosed for further research.

---

## Methodology

### Workflow
1. **App-Based Capture**:
   - A custom app displays patterns and captures images simultaneously on a mobile device.
   
2. **Pattern Learning**:
   - Uses 3D-printed objects and HDR imaging to train the system.
   - Optimized patterns enhance the accuracy of surface normal estimation.

3. **Flexible Deployment**:
   - No specialized equipment or controlled environment is required.
   - Works in general settings with mobile devices.

### Advantages
- No need for a dark room or fixed setup.
- High adaptability to diverse locations and objects.
- Utilizes common mobile devices, reducing hardware dependency.

---

## Results

| Pattern Type       | Reconstruction Error |
|--------------------|----------------------|
| Unlearned Pattern  | **0.07394**         |
| Learned Pattern    | **0.05337**         |

DMDPS achieves accurate surface normal estimation even in uncontrolled environments, demonstrating significant improvement over traditional methods.

---

## Applications
- **Surface Normal Reconstruction**: Enhanced accuracy for real-world objects.
- **Research Database**: Offers a public dataset of surface normals and albedos.
- **Flexible Imaging**: Enables high-quality results using common mobile devices.

---

## Future Work
- Further optimize pattern learning for various mobile devices.
- Expand the database to include more diverse objects and materials.
- Explore additional applications in mobile photometric imaging.

For more details, refer to the [full paper](https://gawoon-ban.github.io/) and project documentation, along with the publicly available dataset on GitHub.

