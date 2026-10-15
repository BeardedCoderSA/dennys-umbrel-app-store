# Container image pins

All runtime images are pinned by tag and immutable multiarch manifest digest.

| Service | Image |
|---|---|
| Coolify dashboard, realtime, terminal and permissions initialization | `ghcr.io/coollabsio/coolify:4.4.6@sha256:7c54f42d64c0d20fed4a8f4561df9018a561fecba9931ed3f64a4f3e0d34a3be` |
| Coolify testing host | `ghcr.io/coollabsio/coolify-testing-host:latest@sha256:88d0826eb8ae8cecb0c49eaaa9e321a7bf81931a48c8492366607eb211371d81` |
| Docker-in-Docker | `docker:28.0.4-dind@sha256:ddb0033088b4fab74881ade341a582e3c6c8021b82377703ba1a6106bd3ded44` |
| PostgreSQL | `postgres:15@sha256:c189d272e4fcdd1ac419adee675d30be3d389c22ee770d593f15819d22a68a0d` |
| Redis | `redis:7.4.7-alpine3.21@sha256:02f2cc4882f8bf87c79a220ac958f58c700bdec0dfb9b9ea61b62fb0e8f1bfcf` |

The upstream testing-host helper currently has no immutable version tag. It is therefore pinned as `latest@sha256:...`; the digest prevents automatic movement.
