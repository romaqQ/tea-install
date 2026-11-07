# tea-install

The one-command installer for tea.

```sh
curl --proto '=https' --tlsv1.2 -fsSL https://github.com/romaqQ/tea-install/releases/download/install-v1/install | bash
```

It asks where to install, signs you in to GitHub once, then installs the latest
accepted tea release after checking it against the digest GitHub recorded.

Installing needs a GitHub account with read access to the private
`romaqQ/tea` repository; this script grants none. Each release is immutable and
its notes carry the script's sha256: to read it first, download `install`,
compare `sha256sum install`, then run `bash install`.
