# 📊 Google Trends Social Media Dashboard with SerpApi + Power BI

This project demonstrates how to integrate **Google Trends data** into **Power BI** using the [SerpApi](https://serpapi.com/) service.  
It includes queries for **regional interest**, **time series analysis**, **short-term keyword performance**, and **related keywords**.

---

## 🚀 How to Use

1. Copy the desired **M Script** into the **Power BI Advanced Editor** (inside Power Query).  
2. Replace the placeholder `"Paste your Key here"` with your **SerpApi API Key**.  
   - Get your API key by signing in at [SerpApi](https://serpapi.com/).  
   - Navigate to the **Account Section** → copy your **API Key**.  
3. Run the query in Power BI to load the data.

---

## 🔑 Notes
- **Keyword Limit:**  
  - GEO_MAP & TIMESERIES → Maximum **5 keywords** (Example: "TikTok, Youtube, Instagram, Twitter, Facebook")
  - RELATED_TOPICS → Maximum **1 keyword**  (Example": "Youtube")
- **Date Range Options (SerpApi):**  
  - `"all"` → All available data  
  - `"today 5-y"` → Past 5 years  
  - `"now 7-d"` → Past 7 days
- **Power BI Parameter:**
  - `"Keywords"` is a Power BI Parameter → you can create it in Power Query to easily change the search terms without editing the script.
  - `"Key"` is also a Parameter → store your SerpApi API key as a parameter for better security & reusability.
  - How to Make Parameter Power BI:
    1. Go to Power Query Editor → Manage Parameters → New Parameter.
    2. Name it Keywords (Text) and Key (Text).
    3. Replace them directly in the query as shown above.

👉 This way, you can quickly swap out keywords or API keys without touching the M script itself.

---

### 📍 1. GEO_MAP Data (Regional Interest)
GEO_MAP → Regional popularity of keywords.
```m
let
    // Define the API endpoint
    apiUrl = "https://serpapi.com/search.json",

    // Define the parameters
    queryParams = [
        engine = "google_trends",
        q = "TikTok, Youtube, Instagram, Twitter, Facebook",
        data_type = "GEO_MAP",
        date = "today 5-y",
        tz = "-330",
        api_key = "Paste your Key here"
    ],

    // Combine the endpoint and parameters
    fullUrl = apiUrl & "?" & Uri.BuildQueryString(queryParams),

    // Make the HTTP request
    response = Web.Contents(fullUrl),

    // Parse the JSON response
    jsonResponse = Json.Document(response),

    // Convert the response to a table
    dataTable = Table.FromRecords({jsonResponse}),

    // Extract the relevant data
    comparedBreakdownByRegion = dataTable{0}[compared_breakdown_by_region]

in
    comparedBreakdownByRegion
```
---

### 📅 2. TIMESERIES Data (All Dates)
TIMESERIES (all) → Long-term interest trend (line/area chart).
```m
let
    // Define the base URL for the API call
    BaseUrl = "https://serpapi.com/search",

    // Define the query parameters with engine, terms, data type, date, and time zone
    QueryParams = [
        engine = "google_trends",
        q = Keywords ,
        data_type = "TIMESERIES",
        date = "all",
        tz = "-330",
        api_key = Key
    ],

    // Generate the full URL with query parameters
    UrlWithParams = BaseUrl & "?" & Text.Combine(List.Transform(Record.FieldNames(QueryParams), 
    each _ & "=" & Uri.EscapeDataString(Record.Field(QueryParams, _))), "&"),

    // Fetch data from the API
    JsonResponse = Json.Document(Web.Contents(UrlWithParams)),

    // Extract the "interest_over_time" part from the JSON response
    InterestOverTime = JsonResponse[#"interest_over_time"]

in
    InterestOverTime
```

---

### 3.📅 TIMESERIES Data (Past 7 Days) <br>
TIMESERIES (7 days) → Short-term interest trend (weekly trend).
```m
let
    // Define the base URL for the API call
    BaseUrl = "https://serpapi.com/search",

    // Define the query parameters
    QueryParams = [
        engine = "google_trends",
        q = Keywords,
        data_type = "TIMESERIES",
        date = "now 7-d",
        tz = "-330",
        api_key = Key
    ],

    // Generate the full URL with query parameters
    UrlWithParams = BaseUrl & "?" & Text.Combine(
        List.Transform(
            Record.FieldNames(QueryParams),
            each _ & "=" & Uri.EscapeDataString(Record.Field(QueryParams, _))
        ),
        "&"
    ),

    // Fetch data from the API
    JsonResponse = Json.Document(Web.Contents(UrlWithParams)),

    // Extract the "interest_over_time" part from the JSON response
    InterestOverTime = JsonResponse[#"interest_over_time"]
in
    InterestOverTime
```

---

### 🔎 4. Related Keywords (Top & Rising) <br>
RELATED_TOPICS → Related keywords, including Rising and Top queries.
```m
let
    // Define the API endpoint
    apiUrl = "https://serpapi.com/search.json",

    // Define the parameters
    queryParams = [
        engine = "google_trends",
        q = "The Developer",
        data_type = "RELATED_TOPICS",
        api_key = "Paste your Key here"
    ],

    // Combine the endpoint and parameters to create the full URL
    fullUrl = apiUrl & "?" & Uri.BuildQueryString(queryParams),

    // Make the HTTP request and get the response
    response = Web.Contents(fullUrl),

    // Parse the JSON response
    jsonResponse = Json.Document(response)
in
    jsonResponse
```
---



