# roguix channel

Roguix's Guix System modules: the Omarchy desktop, the Try Roguix VM
integrations and their packages. They are published here from
[try-roguix](https://github.com/rofrol/try-roguix) (`guest/guix`) by its
`publish-channel` script; edit them there, not here.

A Roguix VM updates with `roguix-update`, which authenticates every commit from
the channel introduction:

```scheme
(channel
 (name 'roguix)
 (url "https://github.com/rofrol/roguix-channel")
 (introduction
  (make-channel-introduction
   "bcc938512706d19de86dd8c6f50853fa80b063b8"
   (openpgp-fingerprint
    "7D1A 8B40 0C26 0998 097F  63E5 28B8 3B16 11FA 815E"))))
```

The modules build on the Guix commit in `modules/roguix/guix-commit`;
binaries for Roguix's own packages come from `https://roguix.frolow.dev`.
