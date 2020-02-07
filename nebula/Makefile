NEBULA_RELEASE:=v1.1.0

all: build push

build:
	docker build --build-arg nebula_release="${NEBULA_RELEASE}" \
		-t cryptorado/nebula:${NEBULA_RELEASE} .

push:
	docker push cryptorado/nebula:${NEBULA_RELEASE}
