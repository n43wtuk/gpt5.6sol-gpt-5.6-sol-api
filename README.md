# GPT-5.6 Sol API (gpt-5.6-sol / gpt5.6sol) — llm guide with published pricing

> **input $3.2; cached_input $0.32; cache_write $4** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-73c322)** · **[Get an API key](https://go.apimart.ai/k-979305)**

Everything here refers to **gpt-5.6-sol** — also written **gpt5.6sol** or **gpt 5.6 sol**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $3.2 |
| `cached_input` | $0.32 |
| `cache_write` | $4 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $320 |
| 1,000 | $3,200 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"gpt-5.6-sol","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
