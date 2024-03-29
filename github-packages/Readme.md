export GH_USERNAME='jacinth54'
export GH_TOKEN=
export GH_IMAGE_NAME='hello-world'
export GH_VER='1.0.0'
export TAG_NAME="ghcr.io/jacinth54/hello-world:1.0.0"

echo $GH_TOKEN | docker login ghcr.io -u $GH_USERNAME --password-stdin

docker tag hello-world:latest ghcr.io/jacinth54/hello-world:1.0.0

docker push ghcr.io/jacinth54/hello-world:1.0.0

to link to a repo: LABEL org.opencontainers.image.source https://github.com/OWNER/REPO