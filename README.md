# Babashka Flatpak

To build and install it:

```sh
# Remove all `--user` to install system-wide

$ flatpak --user install org.flatpak.Builder
$ flatpak --user run org.flatpak.Builder \
    --force-clean \
    --sandbox \
    --user \ # Remove this line to install system-wide
    --install \
    --ccache \
    builddir \
    org.freedesktop.Sdk.Extension.babashka.yaml
```
