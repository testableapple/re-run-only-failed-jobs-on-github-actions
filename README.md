# Specification
- `actions/cache@v2` caches previous result
- `if` condition skips already successful jobs on rerun:

```yml
  if: steps.last_run_status.outputs.last_run_status != 'success'
```
