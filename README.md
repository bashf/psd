Present script directory.

```bash
z="${BASH_SOURCE[0]}"
if [ -h "$z" ]; then z=$(readlink "$z"); fi
cd $(dirname "$0") && cd $(dirname "$z") && pwd
```
