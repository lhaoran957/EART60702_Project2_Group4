# EART60702_Project2_Group4

## Project Title

Predicting Daily Maximum Temperature and Humidity at Manchester

## Project Aim

Predict TREFMXAV_U for January 2050 to December 2080 using a supervised machine learning model.

How does near-surface specific humidity evolve in Manchester from the historical period (2006–2049) to the future projection period (2050–2080), and how does its coupling with temperature influence the frequency of compound hot-humid events?

## Dataset Source

Daily climate model data from **CESM2 LENS2** were used.

- Location: Manchester grid point
- Period: 2006–2080
- Historical period: 2006–2049
- Future period: 2050–2080
- Ensemble members: 003–008

## Variables Used

Main variables:
- `TREFMXAV_U`: daily maximum temperature
- `QBOT`: near-surface specific humidity

Additional variables:
- `TREFHT`
- `FSNS`
- `FLNS`
- `UBOT`
- `VBOT`
- `PRECT`
- `PRSN`

Derived variables:
- `TREFMXAV_U_C`
- `TREFHT_C`
- `QBOT_gkg`
- `sin_doy`
- `cos_doy`
- `year_norm`

## File Structure

- `project 2.ipynb`: main notebook for EDA and machine learning
- `README.md`: project description
- `*.csv`: model results and summary tables
- `*.png`: output figures
- `*.nc`: climate model data files

##Required packages:

- numpy
- pandas
- xarray
- matplotlib
- seaborn
- scipy
- scikit-learn
- netCDF4
- h5netcdf

## Main Findings

- Manchester is projected to become warmer in the future.
- Daily maximum temperature increases, especially in summer.
- Near-surface specific humidity also increases.
- The strongest moistening occurs in the warm season.
- Hotter days tend to be more humid.
- Compound hot-humid days become more frequent after 2050.
- Machine learning models show good predictive skill, although summer humidity is harder to model.
