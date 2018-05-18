# Docker image for opeanapi-spec-validator

Images are based on Python on Alpine and contains only added [openapi-spec-validator](https://github.com/p1c2u/openapi-spec-validator).

Tags are copying validator version.

## Usage

Lets say that your OpenAPI specification is in your current folder in folder `spec` in file `openapi.yaml`. To validate it run

```bash
docker run \
  --rm \
  --volume ${PWD}/spec:/spec \
  zemanlx/openapi-spec-validator:0.2.0 \
  /spec/openapi.yaml
```
