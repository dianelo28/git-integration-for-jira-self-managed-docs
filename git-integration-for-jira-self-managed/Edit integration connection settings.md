---

title: Edit integration connection settings
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# Edit integration connection settings

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1930397536/Edit+integration+connection+settings>

* * *

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930397536/gitcfg-actions-edit-repo-conn-cfg.png?version=1&modificationDate=1630642845462&cacheVersion=1&api=v2&width=680&height=213)

Clicking ![(blue star)](/wiki/s/-1639011364/6452/8b4898d3c114827e64ec143b4fa79bb76a6cfa5b/_/images/icons/emoticons/star_blue.png) Actions ➜ **Edit integration connection settings** opens the configuration page for integration connection settings.

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930397536/gitserver-edit-integration-conn-cfg.png?version=1&modificationDate=1630642844991&cacheVersion=1&api=v2&width=680&height=514)

Utilize the following options to configure the selected integration:

|     |     |
| --- | --- |
| **Option** | **Description** |
| _**Display Name**_ | This is the name that will appear on the Repository/Integration column. |
| _**Personal Access Token**_ | If the PAT has expired or changed, enter the new PAT on the provided box. |
| _**SSL Verify**_ | The Git Integration for Jira app will enforce/ignore verification of SSL certificated when connecting to a git server. For more information, see [SSL verify](/wiki/spaces/GIJDC/pages/1930397639/SSL+verify). |
| _**TrustFolderStat**_ | When this setting is set to `False`, the objects/pack folder will always be scanned to check for new pack files. If set to `True`, the `last-modified` attribute of the folder will be used instead to check the folder for modifications.<br><br>The default value for Jira Server is `True`. For Jira Data Center, it's `False`.<br><br>If your repository is stored on a network share, it is highly recommended to set this option to `False`. |
| _**Custom API Path**_ | The Git Integration for Jira app supports this feature for GitHub and GitLab integrations. For more details, see [Working with Custom API Path](https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/135331922/Working+with+Custom+API+Path). |
| _**JMESPath Filters**_ | JMESPath is a query language for JSON used to filter API results and to limit which repositories are integrated. For more information, see [Working with JMESPath Filters](/wiki/spaces/GIJDC/pages/135430238/Working+with+JMESPath+Filters). |

[« Show tracked or integration repositories](/wiki/spaces/GIJDC/pages/1930397507/Show+tracked+or+integration+repositories)

[Edit integration feature settings »](/wiki/spaces/GIJDC/pages/1930397576/Edit+integration+feature+settings)

### More related topics about managing repository/integration configuration

*   Page:
    
    [Managing repository or integration configuration](/wiki/spaces/GIJDC/pages/1930397435/Managing+repository+or+integration+configuration) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Managing integration via Actions](/wiki/spaces/GIJDC/pages/1930397476/Managing+integration+via+Actions) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Show tracked or integration repositories](/wiki/spaces/GIJDC/pages/1930397507/Show+tracked+or+integration+repositories) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Edit integration connection settings](/wiki/spaces/GIJDC/pages/1930397536/Edit+integration+connection+settings) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Edit integration feature settings](/wiki/spaces/GIJDC/pages/1930397576/Edit+integration+feature+settings) (Git Integration for Jira Data Center)
    
*   Page:
    
    [SSL verify](/wiki/spaces/GIJDC/pages/1930397639/SSL+verify) (Git Integration for Jira Data Center)
    
*   Page:
    
    [View integration or repository properties](/wiki/spaces/GIJDC/pages/1930397673/View+integration+or+repository+properties) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Viewing indexing logs](/wiki/spaces/GIJDC/pages/1930397702/Viewing+indexing+logs) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Removing integration or repository configuration](/wiki/spaces/GIJDC/pages/1930397738/Removing+integration+or+repository+configuration) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Edit repository settings](/wiki/spaces/GIJDC/pages/1947107348/Edit+repository+settings) (Git Integration for Jira Data Center)