# Babashka Flatpak

# Setup

## Prerequisites

- [`org.freedesktop.Sdk.Extension.leiningen`](https://git.sr.ht/~achrinza/org.freedesktop.Sdk.Extension.leiningen)

To build and install it:

```sh
# Remove all `--user` to install system-wide

$ flatpak --user install org.flatpak.Builder
$ flatpak --user run org.flatpak.Builder \
    --force-clean \
    --user \ # Remove this line to install system-wide
    --install \
    --ccache \
    builddir \
    org.freedesktop.Sdk.Extension.babashka.yaml
```

Building with the `--sandbox` flag is not supported.

## License

[FSFAP](./LICENSES/FSFAP)

