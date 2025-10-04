diagrams/mabuhightrack-activity.md
# MabuHighTrack – Activity Diagram

```mermaid
flowchart TD
  A[Start] --> B[Login]
  B --> C{Authenticated?}
  C -- Yes --> D[View Dashboard]
  C -- No --> E[Error Message]
  D --> F[End]
  E --> B
