# matchable

Tiny, type-safe helpers for matching enums, unions, and objects.

## Install
```bash
npm install matchable
```

## Usage
```ts
import { me } from "matchable";

const status = me<"idle" | "loading" | "error">("loading");

const label = status.match({
  idle: () => "Idle",
  loading: () => "Loading",
  _: () => "Error",
});
```

## Build (for publishing)
```bash
npm run build
```
