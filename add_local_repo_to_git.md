## How to push a loca repo to GIt

I'm doing this as a part of the git tutorial assignment.

I've created a Directory Notes under My local Zipfian git directory (not in the precourse one).

Now form this directory i performed 

`> git init`  command

Now in order to add it to my github repos what I have to do is the following:

`> git remote add origin whatever-address-my-repository is .git`

Then i need to commit and push

`> git push -u origin master`

In my case my repo address is https://github.com/carlotorniai

Therefore i run:

`>  git remote add origin https://github.com/carlotorniai .git` from my Notes directory.

Followed by 

`> git push -u origin master`

Interestingly when i run the above two commands I've got the following error.

fatal: https://github.com/carlotorniai/info/refs?service=git-receive-pack not found: did you run git update-server-info on the server?

I discovered that I need to create a repo on GitHub with the same name (in mY case Notes) first.

I did ( from the web Intrface. There is a way to create it using github API from the command line see http://stackoverflow.com/questions/2423777/is-it-possible-to-create-a-remote-repo-on-github-from-the-cli-without-ssh)

Then I need to actually run the following command:

`git remote add origin  https://github.com/carlotorniai/Notes.git`

followed by

`> git push -u origin master`

But it still didn't work. So I ended up removing my local repo.
Checking out the repo from github and recreating and committing my readme  form there.
