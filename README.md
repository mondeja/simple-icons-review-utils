# Usage

These scripts suppose tha:

- You have a directory named `_review` located at `simple-icons` directory root.
- You have `inkscape` installed.
- You are in Linux using Bash.

## Install

1. Install https://github.com/juanfran/svgo-inkscape
2. Clone this repository at `simple-icons/utils`. Use next command from
 `simple-icons` directory root:
```
git clone https://github.com/mondeja/simple-icons-review-utils.git utils
```
3. Install SVGO globally with `npm install -g svgo`

## Scripts
### Start a review for a remote branch

```bash
bash utils/start-review.sh "<ICON NAME>" "<BRANCH USERNAME OWNER>" "<BRANCH NAME>"
```

### Scale icon to 24px size and align to center

```bash
bash utils/inkscape-scale-align-center.sh "<ICON PATH>" "<OUTPUT PATH>" 
```

### Open two icons for compare them manually

```bash
bash utils/inkscape-gui-compare.sh [-c] "<BLACK ICON PATH>" "<RED ICON PATH>"
```

### Query icon dimensions

```bash
bash utils/inkscape-dimensions.sh "<ICON PATH>"
```

## Print differences between icons

```bash
bash utils/diff.sh "<PREVIOUS ICON PATH>" "<NEXT ICON PATH>"
```
