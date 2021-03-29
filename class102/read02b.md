Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.  Its types as:

    Local Version Control
    Centralized Version Control
    Distributed Version Control

Git has a many definitions according  to its using  like:

    Snapshots

    Git is a DVCS that stores data in a file system made up of snapshots.

    Local Operations

    Git mostly relies on local operations because most necessary information can be found in local resources.

    Tracking Changes

    Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

    Loss of Data

    Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

    States

    Files in Git can reside in three main states: committed, modified and staged.

Local Repository Structure

The local Git repository has three components:

    Working Directory: The actual files reside here.
    Index: The area used for staging
    Head: Points to the most recent commit

The Life Cycle of File Status

    After you edit a file, Git flags it as modified because of changes made after the previous commit.
    You stage the modified file.
    Then, you commit staged changes.

 Types of Remote Repositories

    Cloned Repositories

    Seeing Your Remotes

    Adding Remotes

    Fetching

    Pushing

    Renaming/Removing Remotes

Main processes in Branching

    Creating a New Branch

    Switching Branches

    Create a Branch and Checkout

    List Branches

 Types of Merging

    Fast-Forward Merging

    No Fast-forward

    Three-way Merge

    Fetch and Merge

    Merge Conflicts
