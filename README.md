# OpenInfra journey
The journey and the documents I will take as I go through the passage to become an OpenInfra contributor, After a failed trying to contribute to Django project, I have gone deeply into cloud operations and automation tasks and by my past experience as a talented developer and the admiration I have to openstack I have came up with the idea to focus and became a contributor to the sub projects...  
So here we are...

# Accounts
1. Supposedly there is a mailing list or something which I dont have and donts understand what it is...  
2. Git flow Gerrit: There is a highly alien flow of git exclusively for openstack, You need an account to be a part of the process... hosted on [https://review.opendev.org/](https://review.opendev.org/), This is the account you will send your PRs and review process will be done, so add your SSH key in the settings.  
3. Launchpad: You need a [https://launchpad.net/](https://launchpad.net/) account, I think this is used as a issue tracker, And I believe this is the legacy tool and they are moving to something new.
4. Storyboard: This is the new thing for issue tracking [https://storyboard.openstack.org/](https://storyboard.openstack.org/).
5. IRC: Ok this is also very unusual and weird, I just put this link here [http://hexchat.github.io/downloads.html](http://hexchat.github.io/downloads.html).
6. OpenInfra Account: Join to [https://openinfra.dev/](https://openinfra.dev/), And create an indivisual account.

Ok I think these are enough to start next go to next step...

# Git commit messages
Yep it is very heavily instructed to how you may commit something... First we will read this [https://wiki.openstack.org/wiki/GitCommitMessages](https://wiki.openstack.org/wiki/GitCommitMessages), you can summarize it in:
1. The cardinal rule for creating good commits is to ensure there is only one "logical change" per commit.
2. A very good and complement description.
3. You shall respect machine metadata, I think they are auto generated but incase check `Including external references` out in main reference.

At the end I think you shall read the main reference very carefully, and you can see examples seemply by using `git log` on main projects.


# An contribution example on legecy
Randomly found this commit on Masakari:
```
commit 9d1b9e3e9bd2d88749eae279d65149301f3db5a9
Author: sue <sugar-2008@163.com>
Date:   Thu Nov 17 10:26:15 2022 +0800

    Fix notfication stuck into running status when timeout
    
    For instance or process failure workflow, the failure notification
    would stuck into running status if timeout.
    
    Closes-Bug: #1996835
    Change-Id: I61e941ab9dd831369fcc46a132ae2b11c1dd23ba
    (cherry picked from commit 7ec3edda1ada9c2464d79c84b0fd1d1be22f9336)
```
As you can see this closes a bug with ID #1996835, And so when you search it you will find the launchpad bug: [https://bugs.launchpad.net/masakari/+bug/1996835](https://bugs.launchpad.net/masakari/+bug/1996835), And if you mine enough you will find out the Gerrit review tab: [https://review.opendev.org/c/openstack/masakari/+/864807](https://review.opendev.org/c/openstack/masakari/+/864807).  
This is very interesting as you can see contributor just issued the bug on launchpad, and after discussion introduced the fix on Gerrit himself and after review process it was merged into master, and other supported releases... I think I have a general view on openstack contribution.  

# Next steps
Here I am, thinking about how can I create a staging setup, or how I can run Openstack projects simpler, I have some bugs from previous encounters, I can try to replicate them bugs and add their issue or track the old issue related to them, Or I can search in storyboard and track some simple issues...  

For the time being I am going to read more on [https://opendev.org/openstack/contributor-guide](https://opendev.org/openstack/contributor-guide)...  





