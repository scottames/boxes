# boxes

> [!WARNING]
> Deprecated: this repository has been deprecated in favor of
> [github.com/scottames/containers](https://github.com/scottames/containers)

Misc images (boxes) - primarily intended for use with [distrobox](https://github.com/89luca89/distrobox)
or [toolbox](https://containertoolbx.org/).

See [packages](https://github.com/scottames?tab=packages&repo_name=boxes) for full list of images.

## Arch

Usage:

```shell
# distrobox
distrobox create \
  --image ghcr.io/scottames/arch-toolbox:latest \
  --name arch-toolbox
```

```shell
# docker
docker pull ghcr.io/scottames/arch-toolbox:latest
```

## Fedora

Usage:

```shell
# distrobox
distrobox create \
  --image ghcr.io/scottames/fedora-toolbox:latest \
  --name fedora-toolbox
```

```shell
# docker
docker pull ghcr.io/scottames/fedora-toolbox:latest
```

## Verification

All images are signed with sigstore's [cosign](https://docs.sigstore.dev/cosign/overview/)

- To verify the signature download the [cosign.pub key from this repo](cosign.pub) and run:

  ```shell
  cosign verify --key cosign.pub ghcr.io/scottames/<image>
  ```
