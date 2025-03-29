.DEFAULT_GOAL := build

# Create a phony target to always execute the targets and not confuse them with files of same names
.PHONY: fmt vet build

fmt:
	go fmt ./...

vet: fmt
	go vet ./...

build: vet
	go build -o hello

clean: 
# Clean temporary and object files including executable
	go clean
