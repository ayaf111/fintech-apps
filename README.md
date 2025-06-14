This is analyzing customer satisfaction with mobile banking apps by collecting and processing user reviews from the Google Play Store for three Ethiopian banks:Commercial Bank of Ethiopia (CBE),Bank of Abyssinia (BOA), Dashen Bank

# Google Play Store Bank Reviews Scraper

A Python script to collect and preprocess mobile banking app reviews from the Google Play Store for sentiment analysis.

## 📌 Methodology

### 1. Data Collection
- **Target Apps**: 
  - Commercial Bank of Ethiopia (`com.combanketh.mobilebanking`)
  - Bank of America (`com.boa.boaMobileBanking`) 
  - Dashen Bank (`com.dashen.dashensuperapp`)
  
- **Tools Used**:
  - `google-play-scraper` Python library
  - `pandas` for data processing

- **Parameters**:
  ```python
  reviews(
      app_id,
      lang='en',        # English reviews
      country='et',     # Ethiopia 
      count=400,        # 400 reviews per bank
      sort=Sort.NEWEST, # Most recent first
      sleep_milliseconds=1000 # Avoid rate limits
  )
