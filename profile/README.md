<a href="https://amodb.dev">
  <img src="https://raw.githubusercontent.com/AmoDataBase/.github/main/assets/banner.png" alt="amodb, movie and TV metadata API" width="100%">
</a>

# amodb

**Movie and TV metadata API that speaks TMDB v3 and OMDb.** Change the base URL, keep your code.

[Website](https://amodb.dev) · [Docs](https://amodb.dev/docs) · [Quick start](https://amodb.dev/quickstart) · [Pricing](https://amodb.dev/pricing) · [Status](https://amodb.dev/status) · [YouTube](https://www.youtube.com/@amodatabase)

## What you get

- **Drop in for TMDB v3.** Same paths, same query parameters, same JSON. Point your client at `https://api.amodb.dev/3`.
- **OMDb route.** `https://api.amodb.dev/omdb/` takes the usual `i`, `t`, `s`, `type`, `y`, `plot` and `page` parameters and returns OMDb bodies.
- **Extra data.** Ratings, moods, soundtracks, Wikidata facts and cinema showtimes through `append_to_response` or their own endpoints.
- **One plan shape.** Every plan gets all data. Plans differ only in requests per minute. There is no free tier and no trial.
- **Images included.** `https://img.amodb.dev/t/p/{size}/{file}` with TMDB sizes, no key needed.

## Repositories

| Repository | What it is | Install |
|---|---|---|
| [amodb-js](https://github.com/AmoDataBase/amodb-js) | JavaScript and TypeScript client | `npm install amodb` |
| [amodb-python](https://github.com/AmoDataBase/amodb-python) | Python client, sync and async | `pip install amodb` |
| [amodb-php](https://github.com/AmoDataBase/amodb-php) | PHP client | `composer require amodb/amodb-php` |
| [amodb-go](https://github.com/AmoDataBase/amodb-go) | Go client | `go get github.com/AmoDataBase/amodb-go` |
| [amodb-mcp](https://github.com/AmoDataBase/amodb-mcp) | MCP server for Claude, Cursor and VS Code | `npx -y amodb-mcp` |
| [amodb-openapi](https://github.com/AmoDataBase/amodb-openapi) | OpenAPI 3.1 spec, Postman and Insomnia collections | `openapi.yaml` |
| [amodb-examples](https://github.com/AmoDataBase/amodb-examples) | Next.js app, Python CLI, Telegram and Discord bots | `git clone` |

## Quick start

Create a key in your account at [amodb.dev](https://amodb.dev/pricing), then:

```bash
export AMODB_API_KEY=your_32_character_key

# TMDB v3 style
curl "https://api.amodb.dev/3/movie/550?api_key=$AMODB_API_KEY"

# Same call with a bearer header
curl -H "Authorization: Bearer $AMODB_API_KEY" \
  "https://api.amodb.dev/3/search/movie?query=inception"

# OMDb style
curl "https://api.amodb.dev/omdb/?apikey=$AMODB_API_KEY&t=Fight+Club"
```

## Get help

Read [SUPPORT.md](https://github.com/AmoDataBase/.github/blob/main/SUPPORT.md) for where to ask. Report security problems to security@amodb.dev, see [SECURITY.md](https://github.com/AmoDataBase/.github/blob/main/SECURITY.md).
