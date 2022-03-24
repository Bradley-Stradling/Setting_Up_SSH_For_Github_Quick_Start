# ssh_via_repo_for_UT_Cyber

From your system that you ssh to the labs from copy the key for ssh.
```
cat .ssh/is_rsa.pub
```

Go into profile settings on github

![This is an image](https://github.com/Bradley-Stradling/ssh_via_repo_for_UT_Cyber/blob/main/pics/profile_settings.PNG)

And into SSH and PGP keys

![This is an image](https://github.com/Bradley-Stradling/ssh_via_repo_for_UT_Cyber/blob/main/pics/ssh_and_gpg_keys.PNG)

Hit new SSH key and paste in your ssh key - make title memorable to that key/account/system your ssh-ing from.

![This is an image](https://github.com/Bradley-Stradling/ssh_via_repo_for_UT_Cyber/blob/main/pics/new_ssh_key.PNG)

once the key is place we can test

### Test the SSH key:
```
ssh -T git@github.com
```

then we'll grab the repo ssh url

![This is an image](https://github.com/Bradley-Stradling/ssh_via_repo_for_UT_Cyber/blob/main/pics/ssh%20url.PNG)

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
