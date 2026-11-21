# FellowshipNAS apt repository

Signed apt repository for FellowshipNAS updates, served by GitHub Pages at
<https://slackerchris.github.io/fellowship-nas-apt/>.

An installed FellowshipNAS adds this source with the public key shipped in
its image (`/usr/share/keyrings/fellowship-nas.asc`), so Settings → Updates
can install FellowshipNAS fixes alongside Debian's:

```
deb [signed-by=/usr/share/keyrings/fellowship-nas.asc] https://slackerchris.github.io/fellowship-nas-apt trixie main
```

The repository is published by `publish-apt.sh` in the FellowshipNAS source
repository, which signs `Release` with the FellowshipNAS Updates key held
offline on the owner's machine. Only the signed repository is pushed here;
the private key never leaves that machine.
