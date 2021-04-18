# Specification
- `actions/cache@v2` caches the previous run result
- `if` condition skips already successful jobs on re-run:

```yml
  if: steps.run_result.outputs.run_result != 'success'
```
