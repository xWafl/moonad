# Moonad

![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/BlueGhostGH/moonad/Test/develop?logo=github-actions&logoColor=ffffff&style=for-the-badge) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/BlueGhostGH/moonad?logo=code-climate&style=for-the-badge) ![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/BlueGhostGH/moonad?logo=code-climate&style=for-the-badge) ![Code Climate technical debt](https://img.shields.io/codeclimate/tech-debt/BlueGhostGH/moonad?logo=code-climate&style=for-the-badge)

![npm bundle size](https://img.shields.io/bundlephobia/minzip/@blueghost/moonad?logo=npm&style=for-the-badge) ![npm](https://img.shields.io/npm/dw/@blueghost/moonad?color=blue&logo=npm&style=for-the-badge) ![npm](https://img.shields.io/npm/v/@blueghost/moonad?color=black&label=npm%20version&logo=npm&style=for-the-badge) ![npm type definitions](https://img.shields.io/npm/types/@blueghost/moonad?logo=typescript&style=for-the-badge)

![pkgreview.dev Package Ratings](https://img.shields.io/pkgreview/rating/npm/@blueghost/moonad?color=orange&style=for-the-badge)

## Typed Functional Utility Library for TypeScript

### `moonad` brings to the table well-known patterns and features from strongly typed functional languages to TypeScript

```typescript
import { Lazy } from "./Lazy"

const lazyApplier = Lazy.lazy(() => (x: number) => x * 2)

const lazyVal = Lazy.lazy(() => 3)
    .apply(lazyApplier)
    .map(x => x + 1)

console.log(lazyVal.value) // 7
```

### Installation

To install the stable version:

```bash
npm i @blueghost/moonad
```

### Using moonad

To use moonad simply use the following import syntax:

```ts
import { Lazy } from "@blueghost/moonad"
```

#### Documentation

You can find the automatically generated changelog [here](CHANGELOG.md)

The documentation in markdown format can be found [here](./docs/index.md)

#### Contributing

To contribute, check the contribution guide [here](CONTRIBUTING.md)

#### Licence

`moonad` uses the [MIT](LICENSE) licence
