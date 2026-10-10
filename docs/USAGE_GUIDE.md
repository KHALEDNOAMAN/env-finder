# env-finder - Usage Guide

## What It Does
Scans directories recursively to find .env files and display their contents.

## Usage
```bash
python env_finder.py /path/to/project
```

## Use Cases
| Use Case | Command |
|----------|---------|
| Find all .env files | env-finder . |
| Scan specific project | env-finder ~/projects/myapp |
| Audit before deployment | env-finder . --check-secrets |

## Security Tips
- Never commit .env files to git
- Add .env to .gitignore
- Use .env.example for templates (no real values)
- Rotate leaked keys immediately