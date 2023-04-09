## Cross-compile rust projects with docker

### Build image
```console
podman build . -t rust_build_linux_arm64 -f Dockerfile.linuxarm64
```

### Build to linux/arm64 from project directory
```console
podman run --rm -ti -v `pwd`:/app rust_build_linux_arm64
```

