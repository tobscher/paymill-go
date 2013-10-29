# paymill-go

## Description

Wrapper for the [Paymill
API](https://www.paymill.com/en-gb/documentation-3/reference/api-reference/)
version 2. For more information see the
[godocs](http://godoc.org/github.com/Tobscher/paymill-go).

## Supported endpoints

* Clients
* Payments

## Installation

```bash
go get github.com/Tobscher/paymill-go
```

## Usage

### Import

```go
import paymill "github.com/Tobscher/paymill-go"
```

### Create a new API client

```go
paymillPrivateKey := "9bcf69eb04f9b925dac59258efb3d374"
paymillApiClient  := paymill.NewApiClient(paymillPrivateKey)
```

### Create a new payment

```go
paymillClient := nil
paymillToken  := "098f6bcd4621d373cade4e832627b4f6"

payment := paymillApiClient.CreatePayment(paymillToken, paymillClient)
```

## Changelog

Click [here](https://github.com/tobscher/paymill-go/blob/master/CHANGELOG.md) to view the changelog.

## Maintainers

* Tobias Haar (http://github.com/Tobscher)

## License

MIT License. Copyright 2013 Tobias Haar.
