# dryad-sheet

A single-page DRYAD authenticator sheet generator. Everything runs in the browser
(`index.html`); there is no backend.

## Running locally

The page needs the browser's Web Crypto API, which is only available in a secure
context. Opening `index.html` by double-clicking it may not work, so serve it over
`http://localhost` instead.

### With Docker

```sh
docker compose up -d --build
```

Then open <http://localhost:8080>.

- Use a different port: `PORT=9000 docker compose up -d`
- Pick up changes to `index.html`: rerun `docker compose up -d --build`
- Stop: `docker compose down`

The container listens on `127.0.0.1` only, so other machines on your network
can't reach it. This is on purpose: the page generates authenticator material,
and over plain HTTP only `localhost` counts as a secure context.

### Without Docker

Any static file server bound to localhost works, for example:

```sh
python3 -m http.server 8080 --bind 127.0.0.1
```
