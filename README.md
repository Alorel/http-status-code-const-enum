Say no to typos.

`npm install -d xxx`

Basic usage:

```typescript
import {Request, Response} from 'express';
import {HttpStatusCode} from 'http-status-code-const-enum';

function myHandler(req: Request, res: Response) {
  res.status(HttpStatusCode.NO_CONTENT)
    .end();
}
```

Please note that this is a **const enum**, meaning it cannot be used in a pure JavaScript environment and is therefore only suited for TypeScript.
