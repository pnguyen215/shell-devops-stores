.PHONY: run build test tidy deps-upgrade deps-clean-cache

# ==============================================================================
# Running the main application
# Executes the main.go file, useful for development and quick testing
run:
	go run main/main.go

# Building the application
# Compiles the main.go file into an executable, for production deployment
build:
	go build main/main.go

# ==============================================================================
# Module support and testing
# Runs tests across all packages in the project, showing code coverage
test:
	go test -cover ./...

# Cleaning and maintaining dependencies
# Cleans up the module by removing unused dependencies
# Copies all dependencies into the vendor directory, ensuring reproducibility
tidy:
	go mod tidy
	go mod vendor

# Upgrading dependencies
# Updates all dependencies to their latest minor or patch versions
# Cleans up the module after upgrade
# Re-vendors dependencies after upgrade
deps-upgrade:
	# go get $(go list -f '{{if not (or .Main .Indirect)}}{{.Path}}{{end}}' -m all)
	go get -u -t -d -v ./...
	go mod tidy
	go mod vendor

# Cleaning up the module cache
# Removes all items from the Go module cache
deps-clean-cache:
	go clean -modcache
