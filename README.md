# Detection of Phishing Websites Hosted on Free Web Hosting Domains





## Installation
All the required modules are written in Google Collab. You just need to execute the cell in order to install it. Examples: To install the requests module, just execute the below command.

```bash
  !pip install requests
```
## Dataset Creation

I collected phishing URLs from [Phishtank.com](http://data.phishtank.com/data/onlinevalid.csv) and [Openphish.com](https://openphish.com/feed.txt) and legitimate URLs from [expireddomains.com](https://www.expireddomains.net/alexa-top-websites/).  I filtered out free web-hosted domains (FHDs)-based URLs and calculated the [VirusTotal](https://www.virustotal.com/gui/home/url) score for each URL for confirmation about whether it was a phishing or legitimate URL using the code given in the [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/FHD_URL_Filtering_VirusTotal_calculation.ipynb).

## Feature Extraction 

I used 32 features, and the code for extracting values for each feature for every URL is given in the [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/FeatureExtractionPage.ipynb). After all, I created two types of datasets, i.e., [FHD](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/FHD-Dataset.csv) and [Non-FHD](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/Non-FHD%20Dataset.csv) datasets.

## Phishing Detection usng Machine Learning Algorithms
I used several machine learning algorithms like the Random Forest classifier, decision tree, XGBoost, SVC, multilayer layer perceptron, and linear regression and trained both datasets and analyzed the results. The code for the same is given in the [file](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/ModelTrainingPage.ipynb).

## Note 
For a detailed understanding, please go through the [report](https://github.com/Dew-Drops/Phishing-Detection-Project/blob/main/PhishingDetectionReport.pdf).
