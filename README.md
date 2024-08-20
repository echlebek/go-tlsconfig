# go-tlsconfig
Reusable TLS configuration library

`go-tlsconfig` aims to provide data types that work with common
configuration mechanisms, such as flags, configuration files, and
environment variables. The goal is to provide a reusable and uniform
TLS configuration surface.

While some Go programs can use default TLS configuration provided by
the standard library, many need to create their own `*tls.Config`, which
can be error prone and time consuming.

Many operators will want to provide their own CA certificates, or
lock down which versions of TLS are supported, or even restrict which
ciphers are used in certain TLS versions.
