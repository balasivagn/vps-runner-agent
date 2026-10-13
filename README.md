# vps-runner-agent

Release binaries of the vps-runner worker agent. The source is private. Each release lists the source commit, the Go version, the build command and the SHA-256. EC2 workers install a binary only when that hash matches.

## Runner image

`ghcr.io/balasivagn/vps-runner-actions:2.337.0` is built by the `runner-image` workflow from `images/runner/Dockerfile`, a copy of the private repository's runner image. Workers pull it at boot without credentials, so it must never contain secrets. Pin it by digest in configuration.
