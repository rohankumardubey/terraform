# How to run tests

To run them, use:
```
TF_ACC=1 go test -tags=e2e ./internal/cloud/e2e/... -ldflags "-X \"github.com/hashicorp/terraform/version.Prerelease=<PRE-RELEASE>\""
```

### Flags

* Use the `-v` flag for normal verbose mode.
* Use the `-tfoutput` flag to print the terraform output to standard out.
* Use `-ldflags` to change the version Prerelease to what you set. See
[guide](https://www.digitalocean.com/community/tutorials/using-ldflags-to-set-version-information-for-go-applications)
