# Digital-Nao-JAVA-CORE
# Google Search Engine Results API

`/search` API endpoint allows you to scrape the results from Google search engine via our SerpApi service. Head to the **playground** for a live and interactive demo. You can query `https://serpapi.com/search` using a **`GET`** request.

## [API Parameters](http://API Parameters)


| [Search Query](https://serpapi.com/search-api#api-parameters-search-query "Search Query") |||
| :------------ |
| `q` | Required |Parameter defines the query you want to search. You can use anything that you would use in a regular Google search. e.g. inurl:, site:, intitle:. We also support advanced search query parameters such as as_dt and as_eq. See the full list of supported advanced search query parameters.|


| [Geographic Location](http://https://serpapi.com/search-api#api-parameters-advanced-google-parameters "Geographic Location")|||
| :------------ |
| `location` | Optional|Parameter defines from where you want the search to originate. If several locations match the location requested, we'll pick the most popular one. Head to the /locations.json API if you need more precise control. The location and uule parameters can't be used together. It is recommended to specify location at the city level in order to simulate a real user’s search. If location is omitted, the search may take on the location of the proxy.|
|`uule`|Optional|Parameter is the Google encoded location you want to use for the search. uule and location parameters can't be used together.|

|[ Advanced Google Parameters  ](https://serpapi.com/search-api#api-parameters-advanced-google-parameters " Advanced Google Parameters  ")|||
| :------------ |
| `ludocid`  |Optional |Parameter defines the id (CID) of the Google My Business listing you want to scrape. Also known as Google Place ID.   |
|`lsig`   | Optional  | Parameter that you might have to use to force the knowledge graph map view to show up. You can find the lsig ID by using our Local Pack API or Google Local API.lsig ID is also available via a redirect Google uses within Google My Business. |
|`kgmid`   |Optional| Parameter defines the id (KGMID) of the Google Knowledge Graph listing you want to scrape. Also known as Google Knowledge Graph ID. Searches with kgmid parameter will return results for the originally encrypted search parameters. For some searches, kgmid may override all other parameters except start, and num parameters. |

| [Localization](https://serpapi.com/search-api#api-parameters-localization "Localization") |||
| :------------ |
|`google_domain `|Optional| Parameter defines the Google domain to use. It defaults to google.com. Head to the Google domains page for a full list of supported Google domains.|
|`gl`|Optional|Parameter defines the country to use for the Google search. It's a two-letter country code. (e.g., us for the United States, uk for United Kingdom, or fr for France). Head to the Google countries page for a full list of supported Google countries.|
|`hl`|Optional|Parameter defines the language to use for the Google search. It's a two-letter language code. (e.g., en for English, es for Spanish, or fr for French). Head to the Google languages page for a full list of supported Google languages.|
|`lr`|Optional|Parameter defines one or multiple languages to limit the search to. It uses lang_{two-letter language code} to specify languages and / as a delimiter. (e.g., lang_fr/ lang_de will only search french and german pages). head to the google lr languages page for a full list of supported languages.|

|[Advanced Filters](https://serpapi.com/search-api#api-parameters-advanced-filters "Advanced Filters")|||
| :------------ |
|`tbs`|Optional|(to be searched) parameter defines advanced search parameters that aren't possible in the regular query field. (e.g., advanced search for patents, dates, news, videos, images, apps, or text contents).|
|`safe`|Optional|Parameter defines the level of filtering for adult content. It can be set to active or off, by default Google will blur explicit content.|
|`nfpr`|Optional|Parameter defines the exclusion of results from an auto-corrected query when the original query is spelled wrong. It can be set to 1 to exclude these results, or 0 to include them (default). Note that this parameter may not prevent Google from returning results for an auto-corrected query if no other results are available.|
|`filter`|Optional|Parameter defines if the filters for 'Similar Results' and 'Omitted Results' are on or off. It can be set to 1 (default) to enable these filters, or 0 to disable these filters.|
