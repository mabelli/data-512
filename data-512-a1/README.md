# DATA 512: Human Centered Data Science - A1: Data Curation

The goal of this repository is to gather, process, and analyze monthly Wikipedia traffic from Janurary 2008 to August 2020.

## License
Source data is available under the [MIT Licence](LICENSE). <br />
Wikimedia API [Terms of Use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions).

## API Documentation
The data comes from two API endpoints:
1. The Legacy Pagecounts API (collect monthly desktop and mobile traffic data from Janurary 2008 through July 2016). [Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)
2. The Pageviews API (collect monthly desktop, mobile web, and mobile app traffic data from July 2015 through August 2020). [Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

## CSV File Fields Description
| Column                  | Description                                           |
| ------------------------|:-----------------------------------------------------:|
| year                    | Year of the data                                      |
| month                   | Month of the data                                     |
| pagecount_all_views     | Monthly total pageviews from Legacy API               |
| pagecount_desktop_views | Monthly desktop pageviews from Legacy API             |
| pagecount_mobile_views  | Monthly mobile pageviews from Legacy API              |
| pageview_all_views      | Monthly total pageviews from Pageviews API            |
| pageview_desktop_views  | Monthly desktop pageviews from Pageviews API          |
| pageview_mobile_views   | Monthly mobile (web+app) pageviews from Pageviews API |

## Note & Considerations
Pageview API endpoint has an option to filter user traffic from traffic by web crawlers or spiders, while the Legacy Pagecounts API does not.
Thus, the data from Pageview API only includes user traffic, while the data from Legacy Pagecounts API include traffic from user, web crawlers, and spiders.




