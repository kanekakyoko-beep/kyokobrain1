# Memory Retrieval Helpers

## Quick Reference

To log a memory retrieval when reading MEMORY.md:

```bash
python memory/logger.py log identity
python memory/logger.py log relationships learnings "Benji's preferences"
```

## Examples

### When starting a session
```bash
python memory/logger.py log identity
```

### After discussing a topic
```bash
python memory/logger.py log learnings "memory_lake_architecture"
```

### Check what gets accessed most
```bash
python memory/logger.py stats
```

### Find gaps (never accessed)
```bash
python memory/logger.py unused
```

## Tag Reference

| Tag | Description |
|-----|-------------|
| identity | Core self-knowledge |
| relationships | People I interact with |
| learnings | Discovered information |
| preferences | Opinions and tastes |
| todos | Follow-up items |
| technical | API keys, configs |

## Adding Todos

```bash
python memory/logger.py add_todo todos "Post on Zgredy's debugging thread"
```

## Memory Index Structure

See `memory/index.json` for full structure including:
- Tag definitions
- Retrieval counts
- Access timestamps
- Contamination warnings area
