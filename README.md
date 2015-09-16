Funnelcake repacks

= Setup

```
mkdir fcrepack && cd fcrepack
curl https://raw.githubusercontent.com/mozilla/git-repo/master/repo > ./repo
chmod u+x ./repo
./repo init --no-repo-verify -u git@github.com:mozilla-partners/funnelcake-manifest.git
./repo sync
```

= Prereqs

There may be additional software to install prior to creating repacks

= Build

This will build unsigned repacks that you could use to do an initial QA or verify your funnelcake config.

```
cd scripts
python partner-repack.py -v 41.0
```
