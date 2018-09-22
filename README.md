Get Present script directory.

```bash
# Get present script directory.
psd() {
  z="${BASH_SOURCE[0]}"
  if [ -h "$z" ]; then z="$(readlink "$z")"; fi
  cd "$(dirname "$0")" && cd "$(dirname "$z")" && pwd
}
```


[![bashf](https://i.imgur.com/m4p0wKt.jpg)](https://bashf.github.io)
