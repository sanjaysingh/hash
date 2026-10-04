# Hash Generator

Hash Generator computes a hexadecimal digest of text in the browser. The input is not sent to a server.

**Live app:** https://hash.sanjaysingh.net

## What it does

Choose an algorithm, type or paste text, and the digest updates as you type. Copy the result from the page. The selected algorithm is stored in the `algo` query parameter, so a link can reopen the same algorithm.

Algorithms:

- MD5, SHA-1, SHA-256, and SHA-512
- SHA3-224, SHA3-256, SHA3-384, and SHA3-512
- Keccak-256

MD5 and SHA-1 are included for checksums and interoperability. They are not appropriate for new password storage.

## Privacy

Hashing runs locally with vendored CryptoJS and js-sha3. Nothing is uploaded.

## Run locally

Open `index.html` in a browser. Vue, Bootstrap, CryptoJS, and js-sha3 are under `libs/`. No install or build step is required.

## Deploy

Commits that land on `main` deploy to GitHub Pages at https://hash.sanjaysingh.net. Changes reach `main` through a pull request.
