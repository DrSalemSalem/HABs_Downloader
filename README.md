# Retrieve Harmful Algal Blooms Data
- This script is designed to download in situ data related to Harmful Algal Blooms (HABs) from the Akashiwo "red tide" network, managed by the Fisheries Agency of Japan.  
- The script automates the process of finding and retrieving available HABs data within a specified date range and collects Ancillary Data from each station.

## Data Source
- The HABs data are sourced from the [Akashiwo network](https://akashiwo.jp/) of the Fisheries Agency, Japan.

## Targeted Species
- Chattonella
- Total Diatom
- For other species, please contact us: salem.ibrahim@kuas.ac.jp
  
## Dependencies
We recommend creating a new conda environment and installing the required dependencies.

***Installation steps:***
- ***Step 1:*** On Windows open up a Anaconda Prompt, on Linux and MacOS open up a Terminal.

- ***Step 2:*** Create the environment  
```
conda env create -f environment.yml
``` 

- ***Step 3:*** Activate the environment 

```
conda activate HABs_env
```

## Download the code
- **Clone the repository**
```
git clone https://github.com/RS-ML-Hub/HABs_Downloader.git
```

## Script Workflow
***Step 1:*** Configure Dates by editing the **YYYYMMDD_s** and **YYYYMMDD_e** variables in **HABs_Data_Downloader.py** to set the start and end dates.
- **YYYYMMDD_s**: Start date in "YYYY/MM/DD" format. (e.g., "2023/01/01")
- **YYYYMMDD_e**: End date in "YYYY/MM/DD" format.   (e.g., "2023/09/30")

***Step 2:*** Run the script
```
python HABs_Data_Downloader.py
```

***Step 3***  A CSV file named HABs__{YYYYMMDD_s}_{YYYYMMDD_e}.csv (e.g., HABs__20230101_20230930.csv) will be generated in the script's directory.



