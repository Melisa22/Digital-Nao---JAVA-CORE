# Google Search Engine Results API
[![Api](https://serpapi.com/status/google)](https://serpapi.com/status/google)

`/search` API endpoint allows you to scrape the results from Google search engine via our SerpApi service. Head to the **playground** for a live and interactive demo. You can query `https://serpapi.com/search` using a **`GET`** request.

## [API Parameters]([API Parameters](https://serpapi.com/search-api#api-parameters "API Parameters"))

|[Search Query](https://serpapi.com/search-api#api-parameters-search-query "Search Query")  |  |  |
|--|--|--|
|`q`  | Required | Parameter defines the query you want to search. You can use anything that you would use in a regular Google search. e.g. inurl:, site:, intitle:. We also support advanced search query parameters such as as_dt and as_eq. See the full list of supported advanced search query parameters. |

| [Geographic Location](http://https://serpapi.com/search-api#api-parameters-advanced-google-parameters "Geographic Location")  |  |  |
|--|--|--|
| `location` | Optional|Parameter defines from where you want the search to originate. If several locations match the location requested, we'll pick the most popular one. Head to the /locations.json API if you need more precise control. The location and uule parameters can't be used together. It is recommended to specify location at the city level in order to simulate a real user’s search. If location is omitted, the search may take on the location of the proxy.|
| `uule` | Optional|Parameter is the Google encoded location you want to use for the search. uule and location parameters can't be used together.|
