# anythingllm-avx
AnythingLLM for older CPUs (AVX not AVX2)

Workflow to add `engineType = "binary` to the `generator` block in `server/prisma/schema.prisma` and re-builds engine. Should avoid any prisma AVX2 issues.

Note: LanceDB is default and does not support AVX1. I've had success with Qdrant. You can change this in the settings once AnythingLLM has launched.

Package:
`ghcr.io/johnngone/anythingllm-avx:latest`

Full command:
`docker pull ghcr.io/johnngone/anythingllm-avx:latest`
