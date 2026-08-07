# Arquivo.pt CDX(J) Server API — OpenAPI spec

OpenAPI 3.0 description of the CDX(J) Server API exposed by [Arquivo.pt](https://arquivo.pt) at
`/wayback/cdx` (e.g. https://arquivo.pt/wayback/cdx?url=publico.pt), backed by
[pywb](https://github.com/webrecorder/pywb). See [`openapi.yaml`](./openapi.yaml).

## Run Swagger UI locally

```
docker compose up
```

Then open http://localhost:8081 — it serves this repo's `openapi.yaml` directly (including
"Try it out", which sends real requests to `https://arquivo.pt`). Edits to `openapi.yaml` need
just a browser refresh, no restart.

## Hosting

For the "import by URL" links below to work, this repo needs to be pushed to GitHub so the raw file
is reachable at a stable URL:

```
https://raw.githubusercontent.com/arquivo/cdxj-open-api/main/openapi.yaml
```

## View / import the spec

Once the raw URL above resolves, these hosted tools can load it directly via query param — no upload needed:

- **Swagger Editor** (edit + try-it-out):
  `https://editor.swagger.io/?url=https://raw.githubusercontent.com/arquivo/cdxj-open-api/main/openapi.yaml`
- **Swagger UI** (hosted demo instance):
  `https://petstore.swagger.io/?url=https://raw.githubusercontent.com/arquivo/cdxj-open-api/main/openapi.yaml`
- **Redoc** (read-only reference docs):
  `https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/arquivo/cdxj-open-api/main/openapi.yaml`

**Postman** doesn't support a URL query-param link — instead: *Import → Link* and paste the raw URL.
