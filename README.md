# JWT
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/pedroalbanese/jwt/blob/master/LICENSE.md) 
[![GoDoc](https://godoc.org/github.com/pedroalbanese/jwt?status.png)](http://godoc.org/github.com/pedroalbanese/jwt)
[![Go Report Card](https://goreportcard.com/badge/github.com/pedroalbanese/jwt)](https://goreportcard.com/report/github.com/pedroalbanese/jwt)
[![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/pedroalbanese/jwt)](https://golang.org)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/pedroalbanese/jwt)](https://github.com/pedroalbanese/jwt/releases)

### JSON Web Tokens
JSON Web Tokens are an open, industry standard [RFC 7519](https://datatracker.ietf.org/doc/html/rfc7519) method for representing claims securely between two parties. This version only works with HMAC-SHA2 signatures. ECDH_ES variant, consists in the direct use of a shared symmetric key as the Content Encryption Key (CEK) for the block encryption step (recommended). 

<pre>Usage of jwt:
  -alg string
        signing algorithm identifier
  -claim value
        add additional claims. may be used more than once (default {})
  -compact
        output compact JSON
  -debug
        print out all kinds of debug data
  -header value
        add additional header params. may be used more than once (default {})
  -key string
        path to key file or '-' to read from stdin
  -show
        Show header
  -sign string
        path to claims object to sign, '-' to read from stdin
  -verify string
        path to JWT token to verify or '-' to read from stdin</pre>
        
### Examples:
```sh
echo {\"foo\":\"bar\"} | jwt -key secret.txt -sign - | jwt -key secret.txt -verify -
```
or:
```sh
jwt -key secret.txt -claim "foo=bar" -sign + | jwt -key secret.txt -verify -
```
Access [JSON Web Tokens Debugger](https://jwt.io/) and see [GoDoc](https://pkg.go.dev/github.com/pedroalbanese/jwt?utm_source=godoc).

## License

This project is licensed under the MIT License.

##### Copyright (c) 2020-2021 Pedro Albanese - ALBANESE Research Lab
