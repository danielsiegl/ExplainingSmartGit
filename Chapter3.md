# Chapter 3: Git in a nutshell

### Summary
Git is a distributed version control system designed to track changes in source code during software development. Unlike centralized systems, Git allows every developer to have a complete copy of the project history, enabling offline work and improving collaboration. Git is highly efficient at branching and merging, making it ideal for managing multiple versions of a project simultaneously. **It has become the de facto standard for version control** due to its speed, flexibility, and the robust ecosystem around it, including platforms like GitHub, GitLab, Bitbucket ....
All major it companies are heavily invested in git based tools and offerings! (Microsoft, Google, Atlassian, Amazon, ....)
## Outlook
Git is coming to none software engineers sooner than you might expect! 
A) [LieberLieber LemonTree - enabling Git Workflows for UML/SysML Modelers](https://www.lieberlieber.com/lemontree/de/)
B) [Microsoft Integrating it deeply into the OS](https://www.theverge.com/2024/5/21/24161785/microsoft-windows-file-explorer-version-control-7z-tar)
## Git according to Wikipedia
source: https://en.wikipedia.org/wiki/Git
**Git** ([/ɡɪt/](https://en.wikipedia.org/wiki/Help:IPA/English "Help:IPA/English"))[[8]](https://en.wikipedia.org/wiki/Git#cite_note-:0-9) is a [distributed version control](https://en.wikipedia.org/wiki/Distributed_version_control "Distributed version control") [system](https://en.wikipedia.org/wiki/Software_system "Software system")[[9]](https://en.wikipedia.org/wiki/Git#cite_note-FOOTNOTEChaconStraub201429%E2%80%9331-10) that tracks versions of [files](https://en.wikipedia.org/wiki/Computer_file "Computer file"). It is often used to control [source code](https://en.wikipedia.org/wiki/Source_code "Source code") by programmers collaboratively [developing](https://en.wikipedia.org/wiki/Software_development "Software development") [software](https://en.wikipedia.org/wiki/Software "Software").

Design goals of Git include speed, [data integrity](https://en.wikipedia.org/wiki/Data_integrity "Data integrity"), and support for [distributed](https://en.wikipedia.org/wiki/Distributed_computing "Distributed computing"), non-linear workflows — thousands of parallel [branches](https://en.wikipedia.org/wiki/Branching_(version_control) "Branching (version control)") running on different computers.[[10]](https://en.wikipedia.org/wiki/Git#cite_note-kernel_SCM_saga-11)[[11]](https://en.wikipedia.org/wiki/Git#cite_note-integrity_goals-12)[[12]](https://en.wikipedia.org/wiki/Git#cite_note-linusGoogleTalk-13)

Git was created for use in the development of the [Linux kernel](https://en.wikipedia.org/wiki/Linux_kernel "Linux kernel") by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds") and others developing the kernel.[[13]](https://en.wikipedia.org/wiki/Git#cite_note-pro-git-1.2-14)

As with most other distributed version control systems, and unlike most [client–server](https://en.wikipedia.org/wiki/Client%E2%80%93server "Client–server") systems, Git maintains a local copy of the entire [repository](https://en.wikipedia.org/wiki/Repository_(version_control) "Repository (version control)"), a.k.a. repo, with history and version-tracking abilities, independent of [network](https://en.wikipedia.org/wiki/Computer_network "Computer network") access or a central [server](https://en.wikipedia.org/wiki/Server_(computing) "Server (computing)"). A repo is stored on each computer in a standard [directory](https://en.wikipedia.org/wiki/Directory_(computing) "Directory (computing)") with additional, hidden files to provide version control capabilities.[[14]](https://en.wikipedia.org/wiki/Git#cite_note-15) Git provides features to [synchronize](https://en.wikipedia.org/wiki/Synchronization_(computer_science) "Synchronization (computer science)") changes between repos that share history; copied (cloned) from each other. For collaboration, Git supports synchronizing with repos on [remote](https://en.wikipedia.org/wiki/Computer_network "Computer network") machines. Although all repos (with the same history) are peers, developers often use a central server to host a repo to hold an integrated copy.

Git is a [free and open-source software](https://en.wikipedia.org/wiki/Free_and_open-source_software "Free and open-source software") shared under the [GPL-2.0-only license](https://en.wikipedia.org/wiki/GNU_General_Public_License "GNU General Public License").

## Best Practices are using Feature Branches for new capabilities/features#
**Git's flexibility can be both a strength and a challenge**, especially in large-scale deployments where consistency, collaboration, and process adherence are crucial. To address these challenges, best practice workflows like GitFlow and GitHub Flow have been developed. Here’s a brief overview of these workflows:

![](Pasted%20image%2020240826132423.png)
### 1. GitFlow
- **Introduced by**: Vincent Driessen in 2010.
- **Purpose**: Designed to manage complex projects with multiple versions and release cycles.
- **Key Features**:
  - **Main branches**: 
    - `master`: The production-ready code.
    - `develop`: The integration branch for features; it represents the next release.
  - **Supporting branches**:
    - **Feature branches**: Used for developing new features, branched off `develop`.
    - **Release branches**: Created from `develop` when the release is near; final bug fixes and preparations are made here before merging into `master`.
    - **Hotfix branches**: Used for critical fixes in `master` that need to be addressed immediately.
- **Workflow**:
  1. Developers create feature branches from `develop`.
  2. Once a feature is complete, it is merged back into `develop`.
  3. When a release is ready, a release branch is created from `develop` for final adjustments.
  4. After the release is finalized, the release branch is merged into both `master` and `develop`.
  5. Hotfixes are branched off `master`, then merged into both `master` and `develop`.

### 2. GitHub Flow
- **Introduced by**: GitHub.
- **Purpose**: A simpler, more flexible workflow, ideal for continuous delivery and deployment.
- **Key Features**:
  - **Main branch**:
    - `main`: The single production branch (in GitHub, it’s often called `main`).
  - **Feature branches**: Developers create feature branches directly from `main`.
- **Workflow**:
  1. Developers create feature branches from `main`.
  2. Features are developed and tested in these branches.
  3. Once ready, a pull request (PR) is made to merge the feature branch back into `main`.
  4. The PR is reviewed, tested, and then merged into `main`.
  5. Continuous deployment practices often automatically deploy `main` to production after each merge.

### Comparison:
- **GitFlow** is more structured, making it suitable for projects with scheduled releases and multiple versions, like software with different versions or long-term support.
- **GitHub Flow** is simpler and more suited for teams practicing continuous deployment or working on projects where code is frequently and incrementally pushed to production.

Both workflows aim to maintain order and quality in the development process, but the choice between them depends on the project's nature, the team's size, and the deployment strategy.

