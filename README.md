# Effect HTTP API Documentation

An unofficial documentation site for Effect HTTP API, built with [Thally](https://thally.io) as part of Thally's Senior Developer Experience & Documentation Engineer assessment.

**Live site:** https://effect-http-api.thally.app/

## What's included

| Page                    | File                                             |
| ----------------------- | ------------------------------------------------ |
| Introduction            | `src/content/introduction.mdx`                   |
| Quickstart              | `src/content/quickstart.mdx`                     |
| Handle query parameters | `src/content/guides/handle-query-parameters.mdx` |

Navigation is configured in `docs.json`, and site settings are defined in `src/data/site.ts`.

The Effect HTTP API examples were tested with `effect` and `@effect/platform-node` version `4.0.5`.

## Run locally

Requires Node.js 22 or later.

Clone the repository and install its dependencies:

```bash
git clone https://github.com/sundaray/thally-assessment-hemanta.git
cd thally-assessment-hemanta
npm ci
```

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3040](http://localhost:3040).

## Validate

```bash
npx thally check
npm test
npm run build
```

**Known test failure:** `npm test` reports one failing test in `src/lib/__tests__/doc-route-static-params.test.ts`. The test expects API reference pages from the Thally starter, which this documentation site doesn't include. The test belongs to the Thally runtime and has been left unchanged.
