- **Codex WebSocket interruption now preserves conversation continuity.** Handle
  `response.interrupt` immediately, cancel the active upstream request, and emit
  the interrupted response terminal event while retaining completed output for
  the next request. This fixes the mid-conversation `response.create` type error.
