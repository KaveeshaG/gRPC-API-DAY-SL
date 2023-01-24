# "User Management" gRPC Microservice Example
## Prerequisites

* **required** Go **1.19**, _and_
## Tools

Install the following tools:

* **required** Protocol Buffers Compiler, `protoc` (`3.21.9`, version to date):
    * Homebrew: `brew install protobuf`
    * Alpine 3.15: `apk add protobuf-dev protobuf`
    * Ubuntu 21.10: `apt-get install protobuf-compiler libprotobuf-dev`
* **required** `buf` CLI for linting and compiling:
    * `go install github.com/bufbuild/buf/cmd/buf@v1.9.0`
* **required** Protocol Buffer Plugin for Go:
    * `go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28.1`
* **required** gRPC Plugin for Go:
    * `go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2.0`
* **recommended** Code Formatting, `clang-format`, you can use `find . -name '*.proto' | xargs clang-format -i`
    * Homebrew: `brew install clang-format` (`14.0.6`, version to date):
    * Alpine 3.15: `apk add clang-extra-tools`
    * Ubuntu 21.10: `apt-get install clang-format`
* **recommended** gRPC Health Check tester using `grpc-health-probe`:
    * `go install github.com/grpc-ecosystem/grpc-health-probe@v0.4.14`
