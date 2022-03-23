# ssh_via_repo_for_UT_Cyber

From your system that you ssh to the labs from copy the key for ssh.
```
cat .ssh/is_rsa.pub
```

Go into profile settings on github

foo pic here

And into SSH and PGP keys

foo pic here

Hit new SSH key - make title memorable to that key

foo pic here

once the key is place we can test

### Test the SSH key:
```
ssh -T git@github.com
```

then we'll grab the repo ssh url

foo pic here

and we'll go to a folder that we want to clone the repo to and run the below
```
git clone $foo_your_ssh_url$
```

Now try editing a file in your repo directory (try the README) and then do:
```
git add -A
git commit -am "Update README.md"
git push
```
