NEBULA_RELEASE:=v1.1.0

all: build

# note that build also pushes until multi-arch --load works
build:
	docker buildx build \
		--platform linux/arm/v7,linux/arm64,linux/amd64 --push \
		--build-arg nebula_release="${NEBULA_RELEASE}" \
		-t cryptorado/nebula:${NEBULA_RELEASE} .
