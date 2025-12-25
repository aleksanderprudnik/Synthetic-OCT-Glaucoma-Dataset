This synthetic dataset contains 6 clinically accurate OCT-based features for glaucoma classification, created specifically for quick training and evaluation of CNN architectures. It includes:
 
1. RNFL Thickness: 30-105 μm with anatomically correct TSNIT profiles
2. Cup-to-Disc Ratio: 0.1-0.9 with vertical elongation patterns
3. Neuroretinal Rim: Following ISNT rule with focal notching variations
4. Juxtapapillary RNFL: 3.4 mm circular scan patterns with sectoral analysis
5. Optic Nerve Sheath: 5.5-7.5 mm diameter measured at 3mm mark
6. Macular Thickness: 150-350 μm with GCL+IPL variations

Features are stored in HDF5 format, generated using clinically validated parameters. The dataset includes normal and pathological cases, suitable for developing and validating glaucoma classification models.

Labels: Normal, Open-angle, Angle-closure, Normal-tension, and Secondary glaucoma types.
