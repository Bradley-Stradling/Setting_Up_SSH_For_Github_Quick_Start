# ssh_via_repo_for_UT_Cyber

From your system that you ssh to the labs from copy the key for ssh.
```
cat .ssh/is_rsa.pub
```

### Test the SSH key:
```
ssh -T git@github.com
```




Now try editing a file in your repo directory (try the README) and then do:
```
git add -A
git commit -am "Update README.md"
git push
```
