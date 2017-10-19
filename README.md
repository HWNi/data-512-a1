# DATA512 - A1: Data curation 

The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through September 30 2017. The traffic data were collected by using two different [Wikimedia REST API](https://www.mediawiki.org/wiki/REST_API): Pagecounts API and Pageviews API. After the dataset was constructed, a time series plot was generated in Python. 

## Getting Started

If start with running the Jupyter notebook named 'hcds-a1-data-curation.ipynb' if all prerequisites list below are installed.
If not, please first install all the prerequisites list below and then run the 'hcds-a1-data-curation.ipynb'.

### Prerequisites

Python 3.0+
Jupyter Notebook
Pandas
Matploblib
Seaborn

## Using Wikimedia REST API
During data acquisition, user will need to collect data from two different API endpoints, the Pagecounts API and the Pageviews API.

*Pagecounts API* ([Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)) provides access to desktop and mobile traffic data from January 2008 through July 2016.

*Pageviews API* ([Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through September 2017.

## Final data file
*en-wikipedia_traffic_200801-201709.csv*

All the English Wikipedia traffic data processed in this assignment are finally combined into this CSV file with the following headers:
| Column                  | Value         | 
| ----------------------- |:-------------:| 
| year                    | YYYY          | 
| month                   | MM            | 
| pagecounts_all_views    | num_views     | 
| pagecounts_desktop_views| num_views     | 
| pagecounts_mobile_views | num_views     | 
| pageviews_all_views     | num_views     | 
| pageviews_desktop_views | num_views     |
| pageviews_mobile_views  | num_views     |  

###Notice 
*All the traffic data (i.e. number of page counts or views) exclude the traffic by web crawlers or spiders.*
*Values listed as 0 in the table means that the traffic data were not available through Wikimedia REST API for the corresponding time stamp.*

## License 

By using Wikimedia REST API, you agree to Wikimedia's [Terms of Use](https://wikimediafoundation.org/wiki/Terms_of_Use/en) and [Privacy Policy](https://wikimediafoundation.org/wiki/Privacy_policy).


This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
