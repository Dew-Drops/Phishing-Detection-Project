# Detection of Phishing Websites Hosted on Free Web Hosting Domains





## Installation
All the required modules are written in google collab cell. We just need to execute the cell in order to install it. Examples, to install requests module just execute below command.

```bash
  !pip install requests
```
## Dataset Creation

I collected phishing URLS from [Phishtank.com](http://data.phishtank.com/data/onlinevalid.csv) and [Openphish.com](https://openphish.com/feed.txt), legitimate URLs from [Expireddomains](https://www.expireddomains.net/alexa-top-websites/). I filtered out free web hosted domains(FHDs) based URLs and calculated [VirusTotal](https://www.virustotal.com/gui/home/url) score for each URL for the confirmation about it's phishing or legitimate URL  using code given in [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/FHD_URL_Filtering_VirusTotal_calculation.ipynb).

## Feature Extraction 

I used 32 features and the code for extracting value for each feature for every URL is given in [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/FeatureExtractionPage.ipynb). After all I created two type of dataset i.e [FHD](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/fhd_final_dataset.csv) and [Non-FHD](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/non_fhd_final_dataset.csv) datasets.

## Phishing Detection usng Machine Learning Algorithms
I used several machine learning algorithms like Random Forest classifier, Decision tree, XGBoost, SVC, Multilayer layer perceptron and linear regression and trained both the datasets and analysed the results. The code for the same in given in the [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/ModelTrainingPage.ipynb).

## Note 
For detailed understanding, please go through the [Report](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/PhishingDetectionReport17_05_2023_final.pdf).
