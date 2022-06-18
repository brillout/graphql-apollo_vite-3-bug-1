Bug reproduction.

To run it:

```bash
git clone git@github.com:brillout/graphql-apollo_vue-react-bug
cd graphql-apollo_vue-react-bug/
pnpm install
pnpm run build
```

Same as single line (copy paste me):

```bash
git clone git@github.com:brillout/graphql-apollo_vue-react-bug && cd graphql-apollo_vue-react-bug/ && pnpm install && pnpm run build
```

Observe the error:

```
transforming (98) renderer/app.js✘ [ERROR] Could not resolve "react"

    node_modules/.pnpm/@apollo+client@3.6.8/node_modules/@apollo/client/react/hooks/useReactiveVar.js:1:36:
      1 │ import { useEffect, useState } from 'react';
        ╵                                     ~~~~~~~

  You can mark the path "react" as external to exclude it from the bundle, which will remove this
  error.
```
