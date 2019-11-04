## Build Binary

1. `$ export GO111MODULE=on`
2. `$ go mod init github.com/me/simpleApp`
3. `$ go build`
4. `$ rm -rf /tmp/simpleApp`

## Build Tendermint Core

1. `$ cd $GOPATH/src/github.com/tendermint/tendermint`
2. `$ make install`
3. `$ TMHOME="/tmp/simpleApp" tendermint init`

## Run the App

1. `$ ./simpleApp -config "/tmp/simpleApp/config/config.toml"`