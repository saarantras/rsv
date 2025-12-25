Simple supporting analysis for (papername, cite once finalized)

Downloaded `Weekly_Rates_of_Laboratory-Confirmed_RSV_Hospitalizations_from_the_RSV-NET_Surveillance_System_20251224.csv` from https://data.cdc.gov/Public-Health-Surveillance/Weekly-Rates-of-Laboratory-Confirmed-RSV-Hospitali/29hc-w46k/about_data
Citation: “RSV-NET: Respiratory Syncytial Virus Hospitalization Surveillance Network, Centers for Disease Control and Prevention. WEBSITE. Accessed on 2025-12-24”.
Gzipped so a copy can be included in this repo (data are public domain, us govt.)

Conda environment rsvenv, used through this  created with commands

```
conda create -n rsvenv \
  -c conda-forge \
  python=3.11 \
  numpy \
  pandas \
  matplotlib \
  seaborn \
  jupyterlab \
  ipykernel 
```

For reproducability:

```
conda activate rsvenv
conda env export --no-builds > environment.yml
conda env export --from-history > environment_hist.yml
```