# Integration Map

How components connect and what data flows between them.

### Web2-frontend-scaffold --> Http-api

- **Source**: Web2-frontend-scaffold (`5de60226`)
  - Output ports: Frontend App (config)
- **Target**: Http-api (`320c81d6`)
  - Input ports: Request Input (config)

### Http-api --> Transform

- **Source**: Http-api (`320c81d6`)
  - Output ports: Response (config)
- **Target**: Transform (`29cbd0fb`)
  - Input ports: Input (config)

### Transform --> If-else

- **Source**: Transform (`29cbd0fb`)
  - Output ports: Output (config)
- **Target**: If-else (`f297985a`)
  - Input ports: Input (config)

### If-else --> Email-smtp

- **Source**: If-else (`f297985a`)
  - Output ports: True Branch (config), False Branch (config)
- **Target**: Email-smtp (`e944cbf5`)
  - Input ports: Trigger (config)

### Web2-frontend-scaffold --> Variable-store

- **Source**: Web2-frontend-scaffold (`5de60226`)
  - Output ports: Frontend App (config)
- **Target**: Variable-store (`d2396441`)
  - Input ports: Set Value (config)

### Variable-store --> Delay-timer

- **Source**: Variable-store (`d2396441`)
  - Output ports: Value (config)
- **Target**: Delay-timer (`0493472a`)
  - Input ports: Input (config)

### Delay-timer --> Loop-iterator

- **Source**: Delay-timer (`0493472a`)
  - Output ports: After Delay (config)
- **Target**: Loop-iterator (`310f14b1`)
  - Input ports: Input (config)
