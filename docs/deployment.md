# Deployment Guide

## Platform

Render

---

## Deployment Steps

1. Push code to GitHub
2. Create new Web Service on Render
3. Connect GitHub repository
4. Set start command:

```bash
python app.py
```

5. Set environment port automatically

---

## Production Notes

* Uses dynamic port binding
* Logs enabled via Render dashboard
