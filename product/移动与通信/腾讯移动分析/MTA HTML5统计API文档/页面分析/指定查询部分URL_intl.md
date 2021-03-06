### Feature Description
(Page ranking - Query partial URLs) Query the pv\uv\vv\iv data of URL on a daily basis. You can query the format of URLs to be queried in "Page ranking - Real-time/Offline list query".

**API URL:** `http://mta.qq.com/h5/api/ctr_page`
**HTTP request method:** GET.

### Parameters

| Parameter Name | Type | Meaning | Note |
|---------|---------|---------|---------|
| app_id | Integer | App ID | The ID generated during application registration |
| start_date | String | Start time | Start time (Y-m-d) |
| end_date | String | End time | End time (Y-m-d) |
| urls | String | url address | Multiple url addresses are separated with "," and must be URL-encoded |
| idx | String | Metric list | The metric list. Separate query metrics with ",". For available values, please see Appendix (metric dictionary). |
| sign | String | Verification string | See the example of generation process |

### Query Metrics

| Metric | Meaning | Calculation Method |
|---------|---------|---------|
| pv | Number of times that a page has been opened | When a page is opened once, one page view is counted |
| uv | Number of visits per day excluding repeated visits | One unique visit is counted if the page is visited multiple times by the same visitor in a day |
| vv | Number of visits per day | A visitor opens your website until he/she closes all pages and leaves the website, and one visit view is counted |
| iv | Number of IPs used to visit a website in a day | - |
