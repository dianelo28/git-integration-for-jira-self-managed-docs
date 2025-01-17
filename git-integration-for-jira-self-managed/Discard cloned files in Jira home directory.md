---

title: Discard cloned files in Jira home directory
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# Discard cloned files in Jira home directory

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1207828796/Discard+cloned+files+in+Jira+home+directory>

* * *

DEPRECATED

This feature is deprecated and will be removed from the product after August 15, 2022.

This setting is part of the [**General Settings**](/wiki/spaces/GIJDC/pages/966852655/General+Settings) configuration page.

VERSION 4.0.1+ This setting is now moved to the **Advanced settings** in General settings.

  
This feature will reduce Jira server storage by deleting files from cloned git repositories after indexing.  Discarding files can save disk space but may limit some features such as displaying diffs of files.

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1207828796/gencfg-discard-cloned-files.png?version=1&modificationDate=1613125343032&cacheVersion=1&api=v2)

There are three options to choose from:

*   **Keep all cloned binary files. No storage savings. All features available**  This option will leave all cloned repositories intact.
    
*   **Discard all files that match the mask below. Some features limited.**  This option will delete all files in the cloned repositories matching the declared file extensions.
    
*   **Discard all files EXCEPT those that match the mask below. Some features limited.**  This option will delete all other files in the cloned repositories except those files with extensions declared.
    

Select any option with the _discard_ label to enable editing of the file mask field.

Whenever the setting is changed, BigBrassBand recommends to perform a manual reclone of the repositories to ensure an error-free operation.

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