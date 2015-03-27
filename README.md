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

# AUTHOR

Kahlil (Kal) Hodgson <kahlil.hodgson@dealmax.com.au>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2015 by Kahlil (Kal) Hodgson.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
