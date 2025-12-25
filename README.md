Simple supporting analysis of RSV disease burden for (papername, cite once finalized)


# Environment

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

Ran the following to ensure environment is totlly reproducable:

```
conda activate rsvenv
conda env export --no-builds > environment.yml
conda env export --from-history > environment_hist.yml
```

# CDC analysis 

Downloaded hospitaliation data `Weekly_Rates_of_Laboratory-Confirmed_RSV_Hospitalizations_from_the_RSV-NET_Surveillance_System_20251224.csv` from : 

“RSV-NET: Respiratory Syncytial Virus Hospitalization Surveillance Network, Centers for Disease Control and Prevention. WEBSITE. Accessed on 2025-12-24”.
Gzipped so a copy can be included in this repo (data are public domain, us govt.)

Downloaded mortality data `Provisional_Percent_of_Deaths_for_COVID-19,_Influenza,_and_RSV_by_Select_Characteristics_20251225.csv` from : 

National Center for Health Statistics. Provisional Percent of Deaths for COVID-19, Influenza, and RSV by Select Characteristics. Date accessed 2025-12-25. Available from https://data.cdc.gov/Health-Statistics/Provisional-Percent-of-Deaths-for-COVID-19-Influen/53g5-jf7x

Data gzipped to distribute (they are public domain). 

# Havers analysis (not presently used)

Downloaded `zoi241280supp1_prod_1734533637.42786.pdf` from `https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2826104`

Havers FP, Whitaker M, Melgar M, et al. Burden of Respiratory Syncytial Virus–Associated Hospitalizations in US Adults, October 2016 to September 2023. JAMA Netw Open. 2024;7(11):e2444756. doi:10.1001/jamanetworkopen.2024.44756