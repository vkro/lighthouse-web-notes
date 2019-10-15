# Notes for Week 1, Day 1

## Fork and Clone a Gist

> Browse to the gist you'd like to clone

> Click the `Fork` button near the top right corner

You'll be redirected to your own personal fork of this gist

*A fork is a GitHub operation by which one GitHub user creates their own copy of another GitHub user's existing repository or gist.*

> Copy the SSH URL of the gist so that you can clone it.

Once you've selected SSH, copy the URL in the box.

> Clone the gist using the copied USL into your work directory

In Terminal (within Vagrant for the bootcamp), change to the directory you want the clone to live in.

Now clone the URL you copied from the Gist page using the following command (don't copy/paste, make sure you're putting your own SSH URL here):

```shell
git clone git@gist.github.com:YOUR_FORKS_ID.GIT give_the_folder_a_name_here
```

>
Naming your cloned gist directory

Notice that we passed the optional parameter `lunch` to the `git clone` command, after the gist's URL. This is the name we'd like to give our local gist directory. Without specifying it, git clone will automatically create a directory with the name of the gist – in our case the gibberish `7cafdb1e53079cbadb89`.

If you forget to give your gist a more human-readable name (and you haven't made any local changes yet) you can remove the directory (`rm -rf path/to/your/gist/directory` from the Terminal) and `git clone` again, this time passing the optional directory name argument.

>Go to the directory you just created and list the contents to verify that things worked out.
