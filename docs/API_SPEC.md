# Backend API contract

## POST /api/isometric/jobs
multipart/form-data fields:
- image
- prompt
- style
- provider
- demoFallback

Response 202:
```json
{"jobId":"job-id","status":"queued","pollUrl":"/api/isometric/jobs/job-id"}
```

## GET /api/isometric/jobs/:jobId
```json
{
  "jobId":"job-id",
  "status":"completed",
  "progress":100,
  "stage":"completed",
  "attempts":[],
  "result":{
    "imageUrl":"/outputs/result.png",
    "sceneGraph":{},
    "glbUrl":null,
    "provider":"local-procedural",
    "isDemoFallback":true
  }
}
```

## DELETE /api/isometric/jobs/:jobId
Response 202: `{"status":"cancelling"}`

## GET /api/providers/health
Returns configured, healthy, latencyMs and circuit state for every adapter.

## Server-only environment variables
- NANO_BANANA_API_KEY
- DEEPAI_API_KEY
- PIXLR_API_KEY
- CANVA_CLIENT_ID
- CANVA_CLIENT_SECRET
- JOB_SIGNING_SECRET
- STORAGE_BUCKET
- REDIS_URL
