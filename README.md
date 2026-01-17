# LinkedIn Profile Scraper API

A Flask-based REST API that retrieves **public LinkedIn profile URLs** by querying Google Search through **SerpAPI**.
The API is hosted on Render and returns structured, deduplicated LinkedIn profile data based on a given keyword.

---

## 📌 Project Purpose

This project solves the problem of finding LinkedIn professionals **without scraping LinkedIn directly**.

Instead, it:

* Uses Google Search results
* Filters only `linkedin.com/in/` URLs
* Returns clean, usable data for further processing

---

## 🎯 Use Cases

* Lead generation
* Talent sourcing
* Market research
* Healthcare / professional discovery
* Data enrichment pipelines

---

## 🛠 Tech Stack

| Category     | Technology |
| ------------ | ---------- |
| Language     | Python     |
| Framework    | Flask      |
| HTTP Client  | Requests   |
| External API | SerpAPI    |
| Hosting      | Render     |

---

## 🌐 Live API

**Base URL**

```
https://linkedin-scraper-api-atlc.onrender.com
```

**Endpoint**

```
POST /scrape
```

---

## 📥 Request Example

```json
{
  "keyword": "cancer specialists in malakpet",
  "api_key": "YOUR_SERPAPI_KEY"
}
```

---

## 📤 Response Example

```json
{
  "keyword": "cancer specialists in malakpet",
  "pages_scraped": 4,
  "profiles_found": 36,
  "profiles": [
    {
      "name": "Dr XYZ",
      "url": "https://www.linkedin.com/in/example/"
    }
  ]
}
```

---

## 📂 Project Structure

```
.
├── app.py
├── requirements.txt
├── README.md
├── docs/
└── examples/
```

---

## 📖 Documentation

* [Setup Guide](docs/setup.md)
* [Architecture](docs/architecture.md)
* [API Reference](docs/api.md)
* [Deployment](docs/deployment.md)
* [Limitations](docs/limitations.md)

---

## 👨‍💻 Author

**Artham Varshith**
Software Engineer
