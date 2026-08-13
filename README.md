# S-curve

S-кривые строительных проектов (план / прогноз / факт) по данным Jira.

## Содержимое

- `s-curve.html` — HTML-шаблон интерактивной S-кривой
- `scripts/refresh-scurve-jira.py` — обновление данных из Jira и выгрузка HTML
- `canvases/s-curve.canvas.tsx` — Cursor Canvas
- `exports/` — timestamped HTML-снимки

## Выгрузка HTML

```bash
python3 scripts/refresh-scurve-jira.py --export-html
```

Требуется кэш/токен Jira (`JIRA_TOKEN`) для полного обновления; `--export-html` может работать из локального кэша.
