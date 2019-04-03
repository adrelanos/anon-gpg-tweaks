# gnupg configuration for Anonymity Distributions #

Security and privacy enhancements for gnupg's config files
/etc/skel/.gnupg/gpg.conf and /etc/skel/.gnupg/dirmngr.conf.

Ships Thunderbird torbirdy configuration file
/etc/thunderbird/pref/30_whonix.js that allows torified keyserver access.

See also:
https://raw.github.com/ioerror/torbirdy/master/gpg.conf
https://github.com/ioerror/torbirdy/pull/11
## How to install `anon-gpg-tweaks` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org buster main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-gpg-tweaks`.

```
sudo apt-get install anon-gpg-tweaks
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-gpg-tweaks` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`anon-gpg-tweaks` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
