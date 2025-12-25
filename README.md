This synthetic dataset contains 6 clinically accurate OCT-based features for glaucoma classification, created specifically for quick training and evaluation of CNN architectures. It includes:
 
1. RNFL Thickness: 30-105 μm with anatomically correct TSNIT profiles
2. Cup-to-Disc Ratio: 0.1-0.9 with vertical elongation patterns
3. Neuroretinal Rim: Following ISNT rule with focal notching variations
4. Juxtapapillary RNFL: 3.4 mm circular scan patterns with sectoral analysis
5. Optic Nerve Sheath: 5.5-7.5 mm diameter measured at 3mm mark
6. Macular Thickness: 150-350 μm with GCL+IPL variations

Features are stored in HDF5 format, generated using clinically validated parameters. The dataset includes normal and pathological cases, suitable for developing and validating glaucoma classification models.

Labels: Normal, Open-angle, Angle-closure, Normal-tension, and Secondary glaucoma types.

```The HDF5 file contains 3000 total images (500 images per feature) organized as follows:

### Features Group (/features)
1. RNFL Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Range: 30-105 μm
   - Resolution: 224x224 pixels grayscale
   - Clinical patterns: TSNIT profiles, sectoral analysis

2. Cup-to-Disc Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Ratio range: 0.1-0.9
   - Resolution: 224x224 pixels grayscale 
   - Patterns: Vertical elongation, rim variations

3. Rim Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Area range: Following ISNT rule
   - Resolution: 224x224 pixels grayscale
   - Features: Focal notching, diffuse thinning

4. Juxtapapillary Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Scan circle: 3.4mm diameter
   - Resolution: 224x224 pixels grayscale
   - Patterns: Sectoral analysis, wedge defects

5. Sheath Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Diameter range: 5.5-7.5mm
   - Resolution: 224x224 pixels grayscale
   - Measurement: At 3mm mark

6. Macular Input (500 images)
   - Shape: (500, 224, 224, 1)
   - Thickness range: 150-350 μm
   - Resolution: 224x224 pixels grayscale
   - Includes: GCL+IPL variations

### Labels (/labels)
- Shape: (3000, 5)
- One-hot encoded format
- Classes: Normal, Open-angle, Angle-closure, Normal-tension, Secondary

### Metadata Group (/metadata)```
- n_samples: 500 per feature
- feature_names: List of 6 feature types
- datetime_generated: Timestamp of dataset creation
