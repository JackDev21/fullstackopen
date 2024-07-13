```mermaid
sequenceDiagram
    user->>server: HTTP GET /exampleapp/notes
    server-->>user: HTML response (notes page)
    user->>server: HTTP POST /exampleapp/notes (new note data)
    server-->>user: 302 Found (redirect to /exampleapp/notes)
    user->>server: HTTP GET /exampleapp/notes
    server-->>user: HTML response (updated notes page)
