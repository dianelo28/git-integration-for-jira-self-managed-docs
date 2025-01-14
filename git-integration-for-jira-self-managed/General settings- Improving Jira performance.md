---
 
title: General settings - Improving Jira performance
description:
taxonomy:
    category: git-integration-for-jira-self-managed

---

# General settings: Improving Jira performance

<https://bigbrassband.atlassian.net/wiki/spaces/GIJDC/pages/1930396229/General+settings%3A+Improving+Jira+performance>

* * *

**What’s on this page:**

* * *

Access these settings via Jira dashboard menu **Git** ➜ _Manage repositories_ ➜ sidebar **General settings**.

## Improving Git tags performance

Git tags and branches are cached for the most recently viewed 1000 Jira issues (across all Jira projects). The cache is reset each time a new change in any repository is detected. The cache is built the first time an issue with a tag and/or branch is loaded by a user. Subsequent loading of Jira issues with tag or branch information will utilize cached values.

Enabling the display of Git tags in commits for large repositories can affect the performance of Jira. This setting can be disabled by doing the following steps:

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930396229/gitserver-gencfg-git-tags-calc-cfg.png?version=1&modificationDate=1630642785764&cacheVersion=1&api=v2&width=680&height=540)

1.  Go to Jira dashboard menu Git ➜ **Manage repositories**.
    
2.  On your sidebar under Git Integration for Jira, select **General settings**.
    
3.  Under Issue Git integration panel options, uncheck the **Calculate and show Git tags in the Git Integration panel on issue pages** setting.
    
4.  Click **Save** to save and apply the setting.
    

## Improving diff load performance

There's a default limit to the size of files that the diff'er supports which is 16MB. This is to keep a massive file from impacting the Jira server performance too much.

As of **v2.8.5+** of the Git Integration for Jira app, Jira administrators can control over the size of diffs allowed to be displayed in the code diff dialog:

1.  Go Jira dashboard menu Git ➜ **Manage repositories**. On the sidebar under Git Integration for Jira, select **General settings**. Scroll down to **Diff** then set the **Max Diff Line Count** value as desired.  Maximum supported value is 20000.
    

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1930396229/image-20210301-095426.png?version=1&modificationDate=1630642784585&cacheVersion=1&api=v2)

Do note that setting this value higher than the default value will impact the performance when loading the code diff of the selected file in the Git Commits tab. The code diff dialog will truncate the view for each 1500 lines code. To see the rest of the code, manually expand the view.

This setting prevents the display of huge diffs. Thus, improving Jira performance.

## Enable/disable JQL search feature

INTRODUCED VERSION 2.12.0+

On your dashboard menu, go to Git ➜ Manage repositories ➜ **General settings** (sidebar). (Alternatively, go to  ![(blue star)](/wiki/s/-1639011364/6452/8b4898d3c114827e64ec143b4fa79bb76a6cfa5b/_/images/icons/emoticons/star_blue.png) Jira Administration ➜ Applications ➜ **General settings**).

![](https://bigbrassband.atlassian.net/wiki/download/attachments/1930396229/gitserver-gencfg-jql-search-loc2.png?version=1&modificationDate=1630642785286&cacheVersion=1&api=v2)

Enable/disable the JQL searching setting.

This general setting allows administrators to enable/disable the JQL functions within the Git Integration for Jira app.

Turn off this setting to improve Jira performance.

## Smart commits setting

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930396229/gitserver-edit-repocfg-smartcommits.png?version=1&modificationDate=1630642785514&cacheVersion=1&api=v2&width=442&height=91)

To improve performance, turn off smart commits on initial indexing then turn it back on after initial reindexing.

## Commit Notification Emails

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930396229/gitserver-gencfg-email-settings.png?version=1&modificationDate=1630642785995&cacheVersion=1&api=v2&width=680&height=151)

Enable/disable the setting to allow sending of email notifications when a commit is made. This setting defaults to OFF for upgrades and ON for new installation of the Git Integration for Jira app.

Turn off this setting to improve Jira performance.

## Git Activity Stream

![](https://bigbrassband.atlassian.net/wiki/download/thumbnails/1930396229/gitserver-gencfg-git-activity-stream.png?version=1&modificationDate=1630642786223&cacheVersion=1&api=v2&width=544&height=290)

Enable/disable the setting whether to show git commits in the Jira activity stream (Issue page or dashboard widget) or not. For in-place upgrade of the Git Integration for Jira app, this setting is turned off by default.  For new installation, the default setting is enabled.

Disabling this setting will improve Jira performance.

[« New GitLab v10+ authentication](/wiki/spaces/GIJDC/pages/1930396211)

[Adding a repository hosted on Windows Servers or Windows Network share (Admins) »](/wiki/spaces/GIJDC/pages/1930396287)

### More related topics about getting started for git admins

*   Page:
    
    [Setup GitLab Server to respond to incoming network API calls](/wiki/spaces/GIJDC/pages/1930396193/Setup+GitLab+Server+to+respond+to+incoming+network+API+calls) (Git Integration for Jira Data Center)
    
*   Page:
    
    [New GitLab v10+ authentication](/wiki/spaces/GIJDC/pages/1930396211) (Git Integration for Jira Data Center)
    
*   Page:
    
    [General settings: Improving Jira performance](/wiki/spaces/GIJDC/pages/1930396229/General+settings%3A+Improving+Jira+performance) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Adding a repository hosted on Windows Servers or Windows Network Share (Admins)](/wiki/spaces/GIJDC/pages/1930396287) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up repository root not located in Jira Home directory (Admins)](/wiki/spaces/GIJDC/pages/1930396317) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Recommended reindex interval setting](/wiki/spaces/GIJDC/pages/1930396353/Recommended+reindex+interval+setting) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Reindex API to trigger indexing](/wiki/spaces/GIJDC/pages/1930396333/Reindex+API+to+trigger+indexing) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up web linking](/wiki/spaces/GIJDC/pages/1930396395/Setting+up+web+linking) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Setting up webhooks](/wiki/spaces/GIJDC/pages/1930396415/Setting+up+webhooks) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Increasing timeout threshold for large repositories while doing a Git pull](/wiki/spaces/GIJDC/pages/1930396447/Increasing+timeout+threshold+for+large+repositories+while+doing+a+Git+pull) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Working with Tracked folders](/wiki/spaces/GIJDC/pages/1930396479/Working+with+Tracked+folders) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Recommended upgrade method for Git Integration for Jira](/wiki/spaces/GIJDC/pages/1930396509/Recommended+upgrade+method+for+Git+Integration+for+Jira) (Git Integration for Jira Data Center)
    
*   Page:
    
    [Discard cloned files in Jira Home directory (General setting)](/wiki/spaces/GIJDC/pages/1930396547) (Git Integration for Jira Data Center)