# System Architecture

## High-Level Flow

Client → Flask API → SerpAPI → Google Search → LinkedIn URLs → JSON Response

---

## Architecture Overview

1. Client sends keyword and API key
2. Flask API constructs Google search query
3. SerpAPI fetches Google results
4. LinkedIn URLs are filtered and deduplicated
5. Structured JSON response is returned

---

## Design Decisions

* No direct LinkedIn scraping
* Pagination limited to 10 pages
* Rate limiting handled via sleep delays
* Set-based deduplication
