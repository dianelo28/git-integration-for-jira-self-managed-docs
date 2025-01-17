---

title: Git URL ports
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# Git URL ports

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1930396890/Git+URL+ports>

* * *

If your Jira and Git servers are running through a firewall, configure the firewall to allow access using the URL schemes for git repositories. For authentication issues, make sure to check first the correct port for its connection.

Below are the default ports for common git URL protocols:

|     |     |
| --- | --- |
| **Protocol** | **Default Port** |
| ssh:// | port 22 |
| git:// | port 9418 |
| http:// | port 80 |
| https:// | port 443 |

Test git connection and repository URL by doing the following:

1.  Install git client (_or run_ `sudo apt-get install git`)
    
2.  Place your ssh key into `~/.ssh`
    
3.  Clone the repository (or run `git clone <your_repository_url>`)
    

The Git Integration for Jira app will run successfully if the above connection test ran without errors.

[« Working with SSH keys](/wiki/spaces/GIJDC/pages/1930396577/Working+with+SSH+keys)

[Setting up repositories »](/wiki/spaces/GIJDC/pages/1930396906/Setting+up+repositories)