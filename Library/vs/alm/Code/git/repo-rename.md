﻿Title: Rename a Git repository in your team project
Description: ou can rename a Git repository in a few steps, but be aware that your team will have to take a few more steps to adapt to the change.
ms.TocTitle: Rename a Git repo
ms.ContentId: 05971618-4ea9-4997-bb51-2d74211352ef

# Rename a Git repository in your team project

You can rename a Git repository in a team project from your web browser. After you rename the repo, each member of your team will have to take a few steps to re-enable their dev machines to connect to the repo on the server.

## Rename the repo on the server

[!INCLUDE [temp](../_shared/steps-open-control-panel-team-project.md)]

0. Rename the repo from the Version Control tab.

 ![Rename a repository](_img/repo-rename/AdminVC.png)

## Update the Git remotes on your dev machines

Git uses remote references to fetch and push changes between your local copy of a repository and the remote version stored on the server. After a Git repository or team project has been renamed, your remote references need to updated. This is due to the fact that the remote repository URL contains the team project and the repository name. 

Each member of your team must update their local Git repos to continue connecting from their dev machines to the repo in the team project. The instructions below show how to update the remotes for the **Fabrikam Mobile** repo that was renamed to **Fabrikam**.

<a name="copy_remote_repo_url"></a>
### Get the new URL for the repo

Copy the repository URL to your clipboard.

![Git code explorer tab](_img/repo-rename/team-project-git-tabs.png)

![Remote URL for the repository](_img/repo-rename/CloneURL.png)

### Update your remote in Visual Studio 2015

1. Connect to the repo.

 ![Connect to the repository](_img/repo-rename/RepoConnect.png)
 
2. Open the project settings.
 
 ![Project settings](_img/repo-rename/ProjectSettings.png)

3. Open the repo settings.

 ![Repository settings](_img/repo-rename/RepoSettings.png)

4. Edit the fetch and push remote references and paste the URL that you [copied from the remote repo](#copy_remote_repo_url).

 ![Edit remote](_img/repo-rename/EditRepoSettings.png)

### Update your remote in older versions of Visual Studio from the command prompt

If you use an older version of Visual Studio or work with Git from the command prompt:

1. Open the Git command prompt.

2. Go to the local repository and update the remote to the URL you [copied from the remote repo](#copy_remote_repo_url).

    ```git set-url remote origin {URL_you_copied_from_the_remote_repo}```

### Refresh Team Explorer

1. Refresh Team Explorer.

 ![Refresh Team Explorer](_img/repo-rename/RefreshTeamExplorer.png)

2. Team Explorer now shows the updated repo name. 

 ![Team Explorer Updated](_img/repo-rename/Result.png)

## Q&A

<!-- BEGINSECTION class="m-qanda" -->

#### Q: Can I rename my repo again? Can I re-use an old repo name?

A: Yes

#### Q: What if I named my remote something other than the default origin?

A: If you are using:

 * Visual Studio 2015, then edit the remote with the name you used. 

 * An older version of Visual Studio or the command prompt, then run this command: ```git set-url remote {remote_name} {URL_you_copied_from_the_remote_repo}```


<!-- ENDSECTION -->