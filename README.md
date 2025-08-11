# Data Analysis and Visualization Notebook for Image Compression Research

This repository contains the code and data for generating plots and analyzing results for the paper "A Dual Study on Analyzing Image Recompression Effects and Realism Assessment via Kolmogorov Complexity". The notebooks can be accesses: 

- First Part: [Codebase for the first part](https://github.com/elif-ozsoy/Recompression_and_Realism/blob/main/Codebase_First%20Part.ipynb)
- Second Part: [Codebase for the second part](https://github.com/elif-ozsoy/Recompression_and_Realism/blob/main/Codebase_Second%20Part.ipynb)

## Project Structure

- `Codebase_First Part.ipynb`: Main notebook containing the analysis and visualization code
- `Codebase_Second Part.ipynb`: Continuation of the analysis
- Various CSV files containing experimental data
- `Image Realism Files/`: Directory containing additional data files

## Dependencies

Required Python packages:
```
pandas>=1.0.0
matplotlib>=3.0.0
seaborn>=0.11.0
numpy>=1.19.0
matplotlib-inline>=0.1.0
```

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Data Files

The analysis uses several CSV files:
- `heatmap_data.csv`: Data for cross-compression heatmaps
- `*_bitrate_summary.csv`: Files containing PSNR, LPIPS, and FID metrics
- `CRDR_Model*.csv`: Various CRDR model experimental results
- `correlations.csv`: Correlation analysis data
- Additional data files in `Image Realism Files/` directory

## Notebook Contents

The analysis is split across two notebooks that correspond to different sections of the paper:

### Codebase_First Part.ipynb
This notebook implements the analysis for Section 2.3 of the paper, including:

1. **Cross-Compression Analysis** (Section 2.3.2)
   - Heatmap visualization comparing traditional and learned codecs
   - Cross-compression performance analysis

2. **Recompression Analysis** (Section 2.3.3)
   - Rate-distortion curves for learned image compression
   - Multiple recompression cycle analysis
   - Metrics: PSNR, LPIPS, FID

3. **CRDR Analysis** (Section 2.3.4)
   - Impact of bitrate on compression
   - Realism assessment
   - Multiple recompression cycles analysis
   - Configuration comparisons

### Codebase_Second Part.ipynb
This notebook implements the analysis for Section 3 of the paper, focusing on:

1. **Image Realism Assessment** (Section 3.2)
   - Analysis of realism metrics across different datasets
   - Correlation studies with human perception
   - Quality assessment comparisons

2. **Kolmogorov Complexity Analysis** (Section 3.3)
   - Implementation of complexity measures
   - Relationship between compression and realism
   - Cross-dataset validation

### Key Visualizations

The notebook generates several key figures including:
- Cross-compression heatmaps
- Rate-distortion curves
- CRDR model comparisons
- Bitrate vs. quality metrics plots

## Usage

1. Install the required dependencies
2. Ensure all data files are in the correct locations
3. Open and run `Codebase_First Part.ipynb` in Jupyter Notebook or VS Code
4. Cells should be run in sequence as later visualizations depend on earlier computations

## Note

This notebook is part of a larger research project. Make sure all data files are present before running the analysis. The code assumes specific file structures and naming conventions as outlined in the repository structure.
