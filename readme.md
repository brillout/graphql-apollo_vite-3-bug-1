Bug reproduction.

To run it:

```bash
git clone git@github.com:brillout/graphql-apollo_vite-3_bug-1
cd graphql-apollo_vite-3_bug-1/
pnpm install
pnpm run build
```

Same as single line (copy paste me):

```bash
git clone git@github.com:brillout/graphql-apollo_vite-3_bug-1 && cd graphql-apollo_vite-3_bug-1/ && pnpm install && pnpm run build
```

Observe the error:

```
transforming (98) renderer/app.js✘ [ERROR] Could not resolve "react"

    node_modules/.pnpm/@apollo+client@3.6.8/node_modules/@apollo/client/react/hooks/useReactiveVar.js:1:36:
      1 │ import { useEffect, useState } from 'react';
        ╵                                     ~~~~~~~
```

Also observe how the repository doesn't contain the word `react` &mdash; why is `@apollo/client/react` being imported?
