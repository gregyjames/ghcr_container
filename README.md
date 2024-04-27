[![docker_build_push_ghcr](https://github.com/gregyjames/ghcr_container/actions/workflows/tag.yml/badge.svg)](https://github.com/gregyjames/ghcr_container/actions/workflows/tag.yml)
# ghcr_container
Build a docker container and push it to to your private package repo. Using this because I don't want to pay $4.75 a month for a basic azure container repo. For 500mb of storage for free, it's a steal. Especially if you use my [Minimized Go Server Docker Script](https://gist.github.com/gregyjames/f94e85d961f50177da24af722a2a0560), which averages 2.5-3mb per image.

## How to use
Go to settings -> Developer Settings -> Personal Access Tokens -> Tokens (Classic). Create a new token with delete:packages, repo, write:packages permissions. Copy this and save as an repositiory secret named PAT_PACKAGE_TOKEN.

## Azure Container Settings
| Setting    | Value |
| -------- | ------- |
Name | {repo_name}
Image source | Docker Hub or other registries
Image type | Private
Registry login server | ghcr.io
Username | Github Username
Password | PAT_PACKAGE_TOKEN
Image name | {username}/{repo_name}:{version_tag}
