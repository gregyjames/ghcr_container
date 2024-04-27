[![docker_build_push_ghcr](https://github.com/gregyjames/ghcr_container/actions/workflows/tag.yml/badge.svg?branch=main)](https://github.com/gregyjames/ghcr_container/actions/workflows/tag.yml)
# ghcr_container
Build an docker container and push it to to your packages. Using this because I don't want to pay $4.75 a month for a basic azure container repo.

## How to use
Go to settings -> Developer Settings -> Personal Access Tokens -> Tokens (Classic). Create a new token with delete:packages, repo, write:packages permissions. Copy this and save as an repositiory secret named PAT_PACKAGE_TOKEN.

