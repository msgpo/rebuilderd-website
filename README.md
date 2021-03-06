# Arch Linux Rebuilderd Status

A simple status display with the number of reproducible packages for Arch
Linux. Uses rebuilderd's API to fetch the current status of reproducibility.

## Dependencies

* yarn (for building/development)
* caddy (for local development)
* tmux (running watchers)
* ruby-sass

On Arch Linux

```
pacman -S caddy yarn tmux ruby-sass
```

## Development

```
make
./scripts/startdevelop.sh
```

Open http://localhost:8881

## Deployment

Creating a distributable tarball can be done with:

```
make dist
```

## Release

To release a new version:

```
git tag -as v$version
```

Update the rebuilderd-website package in Arch Linux.
