# Reely Mock Backend

This project provides a mock backend for the Reely Automatic Video Captioning Tool frontend, using `json-server` and a sample `db.json` file. It is intended for frontend development and demo purposes only.

---

## Features
- Serves video data via REST API endpoints.
- Simulates video processing statuses (Completed, Processing, Failed).
- Easy to extend or modify for frontend testing.

---

## Getting Started

### 1. Install Dependencies

```
npm install
```

### 2. Start the Mock Backend

```
npm start
```

This runs `json-server` at [http://localhost:8080](http://localhost:8080).

---

## API Endpoints (Only Two)

- `GET /videos` — List all videos
- `GET /videos/:id` — Get details for a specific video

Example response:
```json
{
  "id": 1,
  "title": "Dubai Marina Tour",
  "status": "Completed",
  "createdAt": "2025-07-01",
  "completedAt": "2025-07-02",
  "captionedUrl": "https://example.com/dubai-marina-captioned.mp4"
}
```

---

## Customization
- Edit `db.json` to add or modify video entries.
- Extend endpoints as needed for your frontend.

---

## Notes
- This mock backend does not process videos or perform captioning.
- Use it only for frontend development and demo.

---

## License
MIT
