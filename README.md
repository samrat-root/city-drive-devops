# City Drive – DevOps starter

Run locally:

    docker build -t city-drive .
    docker run --rm -p 8080:8080 city-drive
    # open http://localhost:8080

Pipeline (.github/workflows/ci.yml): lint -> build -> smoke test -> Trivy scan -> push to GHCR (main only).
