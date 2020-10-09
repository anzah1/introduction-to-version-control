# What is version control?

Imagine that you would have access to something that would have following set
of features:

- unlimited undo

- possibility of trying out multiple things at the same time and still having
  having undo for each thing separately

- possibility to see exactly what has been changed

- possibility to work independently and sharing things only when you want to

- possibility to adapt changes from other people when you want to

# What version control is used for?

- main usage is tracking changes in source code

- version control is invaluable tool with development workflow

  - developer can try things out safely while always keeping copy of working
    version of the feature

  - teams can develop features independently

  - whenever there's problem in integration or production environment, version
    control helps tracking down what changed

# Version control is mainly for text

- text is the strongest domain for version control

- binaries are possible, but you'll lose some of the version control features

- with binaries external tools are needed to see what has been changed between
  versions

- for example (old) Word documents are binaries and there's command line tool
  that's able to render them as text

  - more modern Word documents are actually XML files inside a ZIP file, so
    practically they are binaries

# Git

- Git is industry standard version control tool

- Git doesn't try to bundle everything into the installation package

  - that means that few third party tools might be necessary

  - good news is that third party integrations are widely available

  - there are some GUI tools bundled though

- command line version gets all the features first

  - GUI tools are compromises, but for most they implement the most important
    things

  - IDE integration is ideal

# Terms from Git point of view

## commit

- smallest (visible) unit is commit, it contains all changes done to files
  within that commit

- commits are linked together in a chain to create history of changes

## tag

- tag is kind of bookmark into repository

- they're commonly used to mark what commit went into what release

## branch

- branches work like tags, but they have few important differences

  - branches make it possible have non linear history, so relation between
    commits has more tree like structure because branching

  - they can be though of kind of alternate timelines

  - branches very often have common history between each other until they have
    diverged

  - they make working on several features at the same time possible

## merge

- merge is used when two branches are combined together

## repository

- repository houses branches and commits

## clone

- clone will get copy of the repository to your machine

- clone doesn't have to be remote machine, you can also clone repositories from
  your own machine

## push and pull

- push and pull are used to share changes between repositories

- nothing gets automatically shared

# Distributed VS centralized version control

- shift from centralized to distributed version control systems happened quite
  many years ago, but centralized legacy systems might still be out there

- with centralized version control every change is shared with the server

  - that makes it harder to use version control features for trying things out
    in private first

  - communicating with server is slow

  - centralized model is easier to understand though

- before using centralized version control, server needs to be installed first

  - with distributed version control, repository can be created anywhere and
    copied anywhere as needed
