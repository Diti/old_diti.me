---
Description:
  "The “vanity plates” concept, applied to OpenPGP keys, using a program I wrote"
Tags:
- golang
date: 2017-05-11T13:42:54+02:00
title: Un générateur de jolies clés PGP
---

<!-- Introduction here -->

[The `package openpgp` documentation](https://godoc.org/golang.org/x/crypto/openpgp) shows a lot
of frightening functions. But [one of them](https://godoc.org/golang.org/x/crypto/openpgp#NewEntity)
looks [familiar](http://www.dewinter.com/gnupg_howto/english/GPGMiniHowto-3.html#ss3.1):

```go
func NewEntity(name, comment, email string, config *packet.Config) (*Entity, error)
```

I [fiddle with it a bit](https://gist.github.com/Diti/1db81b7e14c2e505a53afb794fac9c1c), trying to
understand how to make use of the library. I think the key…pair is stored in memory.

I’ll need a way to analyse/debug these keys. It would be best if I use *actual* OpenPGP keys for
that, so I fire up `GnuPG`, 