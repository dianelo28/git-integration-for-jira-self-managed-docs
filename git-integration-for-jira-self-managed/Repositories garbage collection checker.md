---

title: Repositories garbage collection checker
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---


# Repositories garbage collection checker

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1207828777/Repositories+garbage+collection+checker>

* * *

These settings are part of the [**General Settings**](/wiki/spaces/GIJDC/pages/966852655/General+Settings) configuration page.

VERSION 4.0.1+ This setting group is now moved to the **Advanced settings** in General settings.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1207828777/gitserver-gencfg-adv-repo-gcc.png?version=1&modificationDate=1647775066834&cacheVersion=1&api=v2&width=680&height=151)

These group of settings control Git repositories garbage collection. Garbage collection process will prune all loose objects, pack loose references and repack all reachable objects into new pack files and remove the old ones.

The higher the change rate of the repository, the more often it would benefit from garbage collection.

This is a block of parameters that determine when the garbage collection task is triggered for the clones of your repositories. The garbage collection task is invoked whenever the number of loose objects or packed files exceeds the set limit.

## Max loose objects count

Set the maximum number of loose objects that will be checked before the garbage collection task is triggered. The garbage collection is activated if the number of loose objects exceeds this setting. Loose objects are individual items that are not compressed into a Git pack file. The recommended default value is _**2000**_.

## Max packed files count

Set the maximum number of packed files that will be checked before the garbage collection is triggered. If the number of packed files count exceeds this setting, the garbage collection is activated. The recommended default value is _**30**_.

* * *

### More on advanced general settings

*   Page:
    
    [Repository settings](/wiki/spaces/GIJDC/pages/1207795977/Repository+settings) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Repositories garbage collection checker](/wiki/spaces/GIJDC/pages/1207828777/Repositories+garbage+collection+checker) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Diff settings](/wiki/spaces/GIJDC/pages/1207795993/Diff+settings) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Discard cloned files in Jira home directory](/wiki/spaces/GIJDC/pages/1207828796/Discard+cloned+files+in+Jira+home+directory) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Git operations timeout](/wiki/spaces/GIJDC/pages/1207828815/Git+operations+timeout) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Smart commits setting](/wiki/spaces/GIJDC/pages/1207828834/Smart+commits+setting) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Cache sizes settings](/wiki/spaces/GIJDC/pages/1207828850/Cache+sizes+settings) (Git Integration for Jira Data Center)