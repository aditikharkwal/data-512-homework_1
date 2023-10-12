# data-512-homework_1

This repository contains analysis of page views of wikipedia articles intended for the Homework 1 for DATA 512 Human Centered Data Science course at the University of Washington - Masters in Data Science program

# Goal of this Project: Reading material on Resources

To learn more about reproducibility I read the following material:

Rokem, Marwick, and Staneva. Assessing Reproducibility in Kitzes, J., Turek, D., & Deniz, F. (Eds.). (2018). The Practice of Reproducible Research: Case Studies and Lessons from the Data-Intensive Sciences. Oakland, CA: University of California Press.

Kitzes. The Basic Reproducible Workflow Template in Kitzes, J., Turek, D., & Deniz, F. (Eds.). (2018). The Practice of Reproducible Research: Case Studies and Lessons from the Data-Intensive Sciences. Oakland, CA: University of California Press.

# Datasource Information

The data for this project is extracted from the wikimedia pageviews API. The pageviews API (documentation) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through the previous complete month. We will make use of this API to extract the page view information.

The following documentation was referred to extract information via API:

Pageviews API Documentation (https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)
Wikimedia Foundation REST API terms of use (https://www.mediawiki.org/wiki/API:REST_API#Terms_and_conditions)

We will follow the following steps to conduct the analysis:

# Tools used

The analysis was conducted in Google Colab. Python was the main language used along with its libraries for the analysis.

# Data Accquisition

We will be using the above mentioned wikimedia API to fetch the pageview data related to the articles listed in the above mentioned excel file. We will store all our data in three files one each for mobile access, desktop access, cumulative views of the articles.

We will aslo store the intermediate data in the folder intermediate_files. These files contain data related to the list of articles we are processing here and the csv formatted response data to enable us manually navigate the data in a tabular format and confirm our findings.

JSON_data/dino_monthly_desktop_201507-202209.json - JSON file containing all articles pages view data for desktop access type JSON_data/dino_monthly_mobile_201507-202209.json - JSON file containing all articles pages view data for mobile access type JSON_data/dino_monthly_cumulative_201507-202209.json - JSON file containing the cumulative page views of all articles for both desktop and mobile access type

# Analysis

The code and steps used for analysis are mentioned in the following file - DATA_512_Assignment_1.ipyb

# Visualizations

We will be using the famous Matplotlib python visualization library here

Figure showing Maximum Average and Minimum Average articles
The first visualization is a time series for the articles that have the highest average page requests and the lowest average page requests for desktop access and mobile access. The graph has four lines (max desktop, min desktop, max mobile, min mobile).

![image](https://github.com/aditikharkwal/data-512-homework_1/assets/38849313/4f9a7fc1-a733-42ff-8574-cdf8187d2e4e)


The second visualization is a time series for the top 10 article pages by largest (peak) page views over the entire time by access type. The graph has the top 10 for desktop and top 10 for mobile access (20 lines).

![image](https://github.com/aditikharkwal/data-512-homework_1/assets/38849313/f18c3d0c-4b62-4234-8f1a-8c3864793e75)

The third visualization is a time series of the articles that have the fewest months of available data. The plot will have relatively short time series, some may only have one month of data. The graph has the 10 articles with the fewest months of data for desktop access and the 10 articles with the fewest months of data for mobile access.

![image](https://github.com/aditikharkwal/data-512-homework_1/assets/38849313/80aac33d-a996-4674-b930-b8c083356c7d)


