# Amorphous-Ice EELS Processing

Python scripts for processing Electron Energy-Loss Spectroscopy Spectrum Imaging (EELS-SI) data stored in Thermo Fisher `.emd` format. These scripts were developed for the analysis presented in our water/ice study.

## Repository Contents

```
Demo/                  # Representative EELS-SI dataset
TEM_env.yaml           # Conda environment
01_*.ipynb             # Read and convert EMD files
02_*.ipynb             # Extract EELS spectra
README.md
LICENSE
```

## Input

- Thermo Fisher `.emd` EELS spectrum imaging data

## Output

The scripts generate:

- `.hspy` files (HyperSpy format)
- `.msa` files (EELS spectra for DigitalMicrograph)

## Demo Dataset

A representative EELS-SI dataset is provided in the `Demo` folder for testing and demonstration purposes.

## Requirements

- Python (recommended via Conda)
- Packages listed in `TEM_env.yaml`
- HyperSpy
- NumPy
- SciPy
- Gatan DigitalMicrograph (GMS) for background subtraction

## Usage

1. Download or clone this repository.
2. Create the Python environment using `TEM_env.yaml`.

```bash
conda env create -f TEM_env.yaml
conda activate TEM_env
```

3. Run the Jupyter notebooks in numerical order.

```
01_...
02_...
```

4. The exported `.msa` files can then be opened in Gatan DigitalMicrograph (GMS) for background subtraction and final visualization.

## Notes

- The notebooks should be executed in numerical order.
- Different notebooks are provided for datasets with different acquisition settings (e.g., 2-, 3-, 4-, or 5-channel acquisitions).
- The scripts were tested using HyperSpy version X.X (optional if you know it).

## Citation

If you use these scripts in your research, please cite:

> Zhang X., et al. *Paper title*. Journal, Year. (Add DOI when available.)

## License

This project is released under the Apache License.
