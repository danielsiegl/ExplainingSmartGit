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

## GitFlow Process using Feature Branches for new capabilities/features#
Git's felxiblity can hinder 

![](Pasted%20image%2020240826132423.png)