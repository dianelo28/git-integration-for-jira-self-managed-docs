---

title: I get the following error - "Host or port specified in are inaccessible". Do I also need a git instance on the Jira server?
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# I get the following error: "Host or port specified in are inaccessible". Do I also need a git instance on the Jira server?

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/2051375166>

* * *

If your Jira and Git servers are running through a firewall, configure the firewall to allow access using the URL schemes for git repositories.  For authentication issues, make sure to check first the correct port for its connection.

Below are the default ports for common git URL protocols:

|     |     |
| --- | --- |
| **Protocol** | **Default port** |
| ssh:// | 22  |
| git:// | 9418 |
| http:// | 80  |
| https:// | 443 |

  
Test git connection and repository URL by doing the following:

1.  Install git client (or run `sudo apt-get install git`)
    
2.  Place your ssh key into `~/.ssh`
    
3.  Clone the repository (or run `git clone <your_repository_url>`)
    

The Git Integration for Jira app will run successfully if the above connection test ran without errors.

*   Page:
    
    [I have an existing git repository on a Jira server. How can I figure out what values should be used for Repository origin and Repository root fields?](/wiki/spaces/GIJDC/pages/2051145752)
    
*   Page:
    
    [Can the app be configured to handle or scan multiple keys for one project? How is this supposed to work?](/wiki/spaces/GIJDC/pages/2052128838)
    
*   Page:
    
    [Where is the location of the local git repository?](/wiki/spaces/GIJDC/pages/2051080265)
    
*   Page:
    
    [How do you configure the Repository Root which is not located in a Jira home directory with Git Integration for Jira?](/wiki/spaces/GIJDC/pages/2052128856)
    
*   Page:
    
    [I get the following error: "Host or port specified in <git\_repository\_url> are inaccessible". Do I also need a git instance on the Jira server?](/wiki/spaces/GIJDC/pages/2051375166)
    
*   Page:
    
    [We use GitBlit without SSH keys and use only HTTPS instead. Does Git Integration for Jira app support this?](/wiki/spaces/GIJDC/pages/2051440710)
    
*   Page:
    
    [I am using Jira which is hosted on Windows. I changed the password of the Active Directory account running Jira. Now, I cannot access my repository. Why?](/wiki/spaces/GIJDC/pages/2051768359)