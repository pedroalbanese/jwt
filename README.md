# JWT
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/pedroalbanese/jwt/blob/master/LICENSE.md) 
[![GoDoc](https://godoc.org/github.com/pedroalbanese/jwt?status.png)](http://godoc.org/github.com/pedroalbanese/jwt)
[![Go Report Card](https://goreportcard.com/badge/github.com/pedroalbanese/jwt)](https://goreportcard.com/report/github.com/pedroalbanese/jwt)
### JSON Web Tokens
JSON Web Tokens are an open, industry standard [RFC 7519](https://datatracker.ietf.org/doc/html/rfc7519) method for representing claims securely between two parties.
<pre>Usage of jwt:
  One of the following flags is required: sign, verify
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
        
## License

This project is licensed under the MIT License.

##### Copyright (c) 2020-2021 Pedro Albanese - ALBANESE Research Lab
