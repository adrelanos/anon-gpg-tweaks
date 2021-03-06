# gnupg configuration for Anonymity Distributions #

Security and privacy enhancements for gnupg's config files
/etc/skel/.gnupg/gpg.conf and /etc/skel/.gnupg/dirmngr.conf.

Ships Thunderbird torbirdy configuration file
/etc/thunderbird/pref/30_whonix.js that allows torified keyserver access.

See also:
https://raw.github.com/ioerror/torbirdy/master/gpg.conf
https://github.com/ioerror/torbirdy/pull/11
## How to install `anon-gpg-tweaks` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-gpg-tweaks`.

```
sudo apt-get install anon-gpg-tweaks
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/anon-gpg-tweaks). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`anon-gpg-tweaks` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
