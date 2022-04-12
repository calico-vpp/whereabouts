build:
	cd ..; ./hack/build-go.sh
image: build
	cp ../bin/whereabouts whereabouts
	go build -o entrypoint entrypoint.go
	docker build -t calicovpp/install-whereabouts .
