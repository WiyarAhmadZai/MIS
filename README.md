<<<<<<< HEAD
# complete MIS
Do cool things!
=======
# attar_hacks

A small Node.js script that generates backdated git commits by repeatedly writing to `data.json` and committing with a custom `--date`.

## Prerequisites

- Node.js (ESM supported)
- Git installed and available on your PATH
- A git repository initialized in this folder
- A configured remote (optional, only if you plan to push)

## Setup

```bash
npm install
```

## Usage

1. Review `index.js` and set the number of commits you actually want to create (the current default is extremely large).
2. Run the script:

```bash
node index.js
```

### What it does

- Writes a timestamp to `data.json`
- Stages and creates a commit with that timestamp as the commit message
- Sets the commit date using git’s `--date` option
- Repeats until the requested count is reached, then pushes

## Notes / Safety

- This will create many commits and can make your repository large and slow.
- Pushing large numbers of commits may take a long time and may be rejected by hosting providers.
- Use this only in repositories where you understand and accept the history you are creating.
>>>>>>> 7a38c5b (Initial commit)
