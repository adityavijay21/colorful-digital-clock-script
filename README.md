# Colorful Digital Clock Script

This Bash script creates a colorful digital clock in the terminal, displaying the current time in green.

## Usage

1. Ensure execution permissions:
   ```bash
   chmod +x colorful_clock.sh
   ```

2. Run the script:
   ```bash
   ./colorful_clock.sh
   ```

## Customization

Modify `Red`, `Green`, and `Blue` variables to change text colors.

```bash
Red=$'\e[1;31m'
Green=$'\e[1;32m'
Blue=$'\e[1;34m'
```

## Example

```bash
#!/bin/bash

Red=$'\e[1;31m'
Green=$'\e[1;32m'
Blue=$'\e[1;34m'

while true; do
    clear
    echo $Green $(date +%T)
    sleep 1s
done
```

## License

This script is provided under the [MIT License](LICENSE).

---
