# API Documentation

## POST /scrape

### Description

Fetches public LinkedIn profile URLs related to a keyword.

---

### Request

**Headers**

```
Content-Type: application/json
```

**Body**

```json
{
  "keyword": "software engineers in bangalore",
  "api_key": "YOUR_SERPAPI_KEY"
}
```

---

### Responses

#### 200 OK

Returns profiles list

#### 400 Bad Request

* Missing keyword
* Missing API key
* Invalid JSON
