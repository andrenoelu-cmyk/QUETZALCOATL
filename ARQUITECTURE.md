[[IDENTITY]]
                    USER
                      │
                      ▼
                   CLI / TUI
                      │
                      ▼
              QUETZALCOATL CORE
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
       TASKS        FILES       SYSTEM
          │           │           │
          ▼           ▼           ▼
       SQLite       Python      Linux
                      │
                      ▼
                   OLLAMA
                  
				   Pero con una distinción fundamental:

```
             OLLAMA
                │
         "quiero hacer X"
                │
                ▼
       TOOL VALIDATION
                │
                ▼
          PERMISSION
                │
        ┌───────┴───────┐
        ▼               ▼
     allowed         confirmation
        │               │
        └───────┬───────┘
                ▼
             TOOL
                ▼
             RESULT
                ▼
             OLLAMA
```