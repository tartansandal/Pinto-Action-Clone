# NAME

App::Pinto::Command::clone - clone a new stack from a different repository

# VERSION

version 0.001

# SYNOPSIS

    pinto --root=REPOSITORY_ROOT clone [OPTIONS] UPSTREAM TO_STACK

# DESCRIPTION

This command creates a new stack by cloning a stack on an upstream repository.
The new stack must not already exist.

Use the [new](https://metacpan.org/pod/App::Pinto::Command::new) command to create a new empty
stack, or the [props](https://metacpan.org/pod/App::Pinto::Command::props) command to change
a stack's properties after it has been created.

# COMMAND ARGUMENTS

The two required arguments are the URL of stack on the upstream repository and target
stack.  The URL could be something like:

    https://www.stratopan.com/thaljef/OpenSource/pinto-release 

Stack names must be alphanumeric plus hyphens, underscores, and periods, and
are not case-sensitive.

# COMMAND OPTIONS

- --default

    Also mark the new stack as the default stack.

- --description=TEXT
- -d TEXT

    Use TEXT for the description of the stack.  If not specified, defaults
    to 'Clone of stack UPSTREAM'.

- --lock

    Also lock the new stack to prevent future changes.  This is useful for
    creating a read-only "tag" of a stack.  You can always use the
    [lock](https://metacpan.org/pod/App::Pinto::Command::lock) or
    [unlock](https://metacpan.org/pod/App::Pinto::Command::unlock) commands at a later time.

# SUPPORT

## Perldoc

You can find documentation for this module with the perldoc command.

    perldoc App::Pinto::Command::clone

## Websites

The following websites have more information about this module, and may be of help to you. As always,
in addition to those websites please use your favorite search engine to discover more resources.

- MetaCPAN

    A modern, open-source CPAN search engine, useful to view POD in HTML format.

    [http://metacpan.org/release/Pinto-Action-Clone](http://metacpan.org/release/Pinto-Action-Clone)

- Search CPAN

    The default CPAN search engine, useful to view POD in HTML format.

    [http://search.cpan.org/dist/Pinto-Action-Clone](http://search.cpan.org/dist/Pinto-Action-Clone)

- RT: CPAN's Bug Tracker

    The RT ( Request Tracker ) website is the default bug/issue tracking system for CPAN.

    [https://rt.cpan.org/Public/Dist/Display.html?Name=Pinto-Action-Clone](https://rt.cpan.org/Public/Dist/Display.html?Name=Pinto-Action-Clone)

- AnnoCPAN

    The AnnoCPAN is a website that allows community annotations of Perl module documentation.

    [http://annocpan.org/dist/Pinto-Action-Clone](http://annocpan.org/dist/Pinto-Action-Clone)

- CPAN Ratings

    The CPAN Ratings is a website that allows community ratings and reviews of Perl modules.

    [http://cpanratings.perl.org/d/Pinto-Action-Clone](http://cpanratings.perl.org/d/Pinto-Action-Clone)

- CPAN Forum

    The CPAN Forum is a web forum for discussing Perl modules.

    [http://cpanforum.com/dist/Pinto-Action-Clone](http://cpanforum.com/dist/Pinto-Action-Clone)

- CPANTS

    The CPANTS is a website that analyzes the Kwalitee ( code metrics ) of a distribution.

    [http://cpants.cpanauthors.org/dist/Pinto-Action-Clone](http://cpants.cpanauthors.org/dist/Pinto-Action-Clone)

- CPAN Testers

    The CPAN Testers is a network of smokers who run automated tests on uploaded CPAN distributions.

    [http://www.cpantesters.org/distro/P/Pinto-Action-Clone](http://www.cpantesters.org/distro/P/Pinto-Action-Clone)

- CPAN Testers Matrix

    The CPAN Testers Matrix is a website that provides a visual overview of the test results for a distribution on various Perls/platforms.

    [http://matrix.cpantesters.org/?dist=Pinto-Action-Clone](http://matrix.cpantesters.org/?dist=Pinto-Action-Clone)

- CPAN Testers Dependencies

    The CPAN Testers Dependencies is a website that shows a chart of the test results of all dependencies for a distribution.

    [http://deps.cpantesters.org/?module=App::Pinto::Command::clone](http://deps.cpantesters.org/?module=App::Pinto::Command::clone)

## Bugs / Feature Requests

[https://github.com/tartansandal/Pinto/issues](https://github.com/tartansandal/Pinto/issues)

## Source Code

The code is open to the world, and available for you to hack on. Please feel free to browse it and play
with it, or whatever. If you want to contribute patches, please send me a diff or prod me to pull
from your repository :)

[https://github.com/tartansandal/Pinto](https://github.com/tartansandal/Pinto)

    git clone git://github.com/tartansandal/Pinto.git

# AUTHOR

Kahlil (Kal) Hodgson <kahlil.hodgson@dealmax.com.au>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2015 by Kahlil (Kal) Hodgson.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
