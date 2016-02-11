getpubkeys
==========

Get a user's public keys from the GitHub API
#####Dependencies:
None! This script only uses the Python standard library


##### Example Usage:
######Look up public keys for GitHub user egalano
```
./getpubkeys egalano
```

######Look up public keys for thatch
```
./getpubkeys thatch
```

######Look up egalano's public keys from a GitHub Enterprise appliance
```
./getpubkeys -a https://my-github.your-company.com egalano
```

######Insecure one-liner to add an existing user's keys to their .ssh/authorized_keys
```
curl -sL https://raw.githubusercontent.com/egalano/getpubkeys/master/getpubkeys | python - egalano >> ~eg/.ssh/authorized_keys
```
