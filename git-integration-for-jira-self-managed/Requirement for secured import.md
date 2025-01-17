---

title: Requirement for secured import
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# Requirement for secured import

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1930397869/Requirement+for+secured+import>

* * *

SSH INTEGRATION

Before adding repositories (new or existing) via Bulk change, make sure that you have added SSH keys for the respective git hosts in the Git Integration for Jira app configuration page. For example, you have GitHub and GitLab repositories to import, add the private SSH keys to the Git for Integration Jira app ➜ **SSH Keys** (_sidebar_) for each git host. For more information, see [Documentation – Adding a private SSH key](/wiki/spaces/GIJDC/pages/1930396698/Adding+a+private+SSH+key).  

HTTP/HTTPS INTEGRATION

If you use HTTP/HTTPS URLs in the origin field, the Git Integration for Jira app will not be able to import said repositories due to missing credentials. Entering repository login credentials in the TSV file is not advisable due to a possible security risk. Therefore, when editing the _**origin**_ field of the TSV file, enter value using the `git@<repository-url>:[your-git-repo].git` format. This format will use the SSH key(s) from the Git Integration for Jira app configuration instead.

  
Proceed to import repositories by following on the next topic.

[« Exporting repository configuration via Bulk change](/wiki/spaces/GIJDC/pages/1930397830/Exporting+repository+configuration+via+Bulk+change)

[Import existing repositories via Bulk change »](/wiki/spaces/GIJDC/pages/1930397888/Import+existing+repositories+via+Bulk+change)

### More related topics about Bulk change

*   Page:
    
    [Bulk change](/wiki/spaces/GIJDC/pages/1930397801/Bulk+change) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Exporting repository configuration via Bulk change](/wiki/spaces/GIJDC/pages/1930397830/Exporting+repository+configuration+via+Bulk+change) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Requirement for secured import](/wiki/spaces/GIJDC/pages/1930397869/Requirement+for+secured+import) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Import existing repositories via Bulk change](/wiki/spaces/GIJDC/pages/1930397888/Import+existing+repositories+via+Bulk+change) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Import new repositories via Bulk change](/wiki/spaces/GIJDC/pages/1930397912/Import+new+repositories+via+Bulk+change) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Editing existing repository settings in the TSV File](/wiki/spaces/GIJDC/pages/1930397941/Editing+existing+repository+settings+in+the+TSV+File) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Removing existing repositories via Bulk change](/wiki/spaces/GIJDC/pages/1930397978/Removing+existing+repositories+via+Bulk+change) (Git Integration for Jira Data Center)