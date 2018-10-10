## Go

These settings apply only when `--go` is specified on the command line.

``` yaml $(go)
go:
  license-header: MICROSOFT_APACHE_NO_VERSION
  namespace: redis
  clear-output-folder: true
```

### Go multi-api

``` yaml $(go) && $(multiapi)
batch:
  - tag: package-2018-03
  - tag: package-2017-10
  - tag: package-2017-02
  - tag: package-2016-04
  - tag: package-2015-08
```

### Tag: package-2018-03 and go

These settings apply only when `--tag=package-2018-03 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2018-03' && $(go)
output-folder: $(go-sdk-folder)/services/redis/mgmt/2018-03-01/redis
```


### Tag: package-2017-10 and go

These settings apply only when `--tag=package-2017-10 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2017-10' && $(go)
output-folder: $(go-sdk-folder)/services/redis/mgmt/2017-10-01/redis
```


### Tag: package-2017-02 and go

These settings apply only when `--tag=package-2017-02 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2017-02' && $(go)
output-folder: $(go-sdk-folder)/services/redis/mgmt/2017-02-01/redis
```

### Tag: package-2016-04 and go

These settings apply only when `--tag=package-2016-04 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2016-04' && $(go)
output-folder: $(go-sdk-folder)/services/redis/mgmt/2016-04-01/redis
```

### Tag: package-2015-08 and go

These settings apply only when `--tag=package-2015-08 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2015-08' && $(go)
output-folder: $(go-sdk-folder)/services/redis/mgmt/2015-08-01/redis
```