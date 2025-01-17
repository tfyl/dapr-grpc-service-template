# dapr-grpc-service-template [![Go Report Card](https://goreportcard.com/badge/github.com/dapr-templates/dapr-grpc-service-template)](https://goreportcard.com/report/github.com/dapr-templates/dapr-grpc-service-template)

### template usage

* Click "Use this template" above and follow the wizard to select owner and name your new repo
* Clone and navigate to your new repo (`git clone <url>>`)
* Initialize your project to set the package names and update imports (`make init`) or (`make init-vendor`)
* Write your subscription event handling logic


### common operations

Common operations to help you bootstrap a Dapr gRPC services development in `go`:

```shell
$ make
init                           Resets go modules and sets up k8s/deployments.yaml
init-vendor                    Resets go modules and sets up k8s/deployments.yaml and initialises go vendor
tidy                           Updates the go modules
tidy-vendor                    Updates the go modules and vendors all dependencies
test                           Tests the entire project
run                            Runs uncompiled code in Dapr
build                          Builds local release binary
invoke                         Invoke service with sample JSON content using Dapr API
image                          Builds and publish docker image
lint                           Lints the entire project
tag                            Creates release tag
clean                          Cleans up generated files
help                           Display available commands
```

This project also includes GitHub actions in [.github/workflows](.github/workflows) that test on each `push` and build images and mark release on each `tag`. Other Dapr GitHub templates to accelerate Dapr development available [here](https://github.com/dapr/go-sdk/tree/master/service).

### License

This software is released under the [MIT](./LICENSE)
