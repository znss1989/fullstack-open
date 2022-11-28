```mermaid
sequenceDiagram
note over Browser: submit data via the form, prevent default redirection
note over Browser: update local notes, update DOM tree
Browser->>Server: HTTP POST /exampleapp/new_note_spa (payload in JSON)
note over Server: Update data on server with new note
Server-->>Browser: 201 Created
``` 