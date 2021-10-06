# Task::FFIDev ![static](https://github.com/PerlFFI/Task-FFIDev/workflows/static/badge.svg) ![linux](https://github.com/PerlFFI/Task-FFIDev/workflows/linux/badge.svg)

Task bundle for FFI development

# SYNOPSIS

```
$ cpanm Task::FFIDev
```

# DESCRIPTION

This [Task](https://metacpan.org/pod/Task) bundle is useful for those doing FFI development with [FFI::Platypus](https://metacpan.org/pod/FFI::Platypus).  Installing it
will give you these modules:

- [Dist::Zilla::MintingProfile::FFI](https://metacpan.org/pod/Dist::Zilla::MintingProfile::FFI)

    [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) minting profile for creating [FFI::Platypus](https://metacpan.org/pod/FFI::Platypus) bindings.

- [Dist::Zilla::Plugin::FFI](https://metacpan.org/pod/Dist::Zilla::Plugin::FFI)

    [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) plugins useful for FFI

- [Dist::Zilla::Plugin::DynamicPrereqs](https://metacpan.org/pod/Dist::Zilla::Plugin::DynamicPrereqs)

    [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) plugin for dynamic prereqs.  Allows your FFI to use [Alien](https://metacpan.org/pod/Alien)s in fallback mode.

- [FFI::C](https://metacpan.org/pod/FFI::C)

    Create interfaces to C structured data.

- [FFI::CheckLib](https://metacpan.org/pod/FFI::CheckLib)

    Find dynamic libraries for use with FFI

- [FFI::Platypus](https://metacpan.org/pod/FFI::Platypus)

    Library for writing your own FFI bindings in perl

- [FFI::Platypus::Type::Enum](https://metacpan.org/pod/FFI::Platypus::Type::Enum)

    Platypus type plugin for enumerated types

- [FFI::Platypus::Type::PtrObject](https://metacpan.org/pod/FFI::Platypus::Type::PtrObject)

    Platypus type plugin for opaque pointer objects

- [PeekPoke::FFI](https://metacpan.org/pod/PeekPoke::FFI)

    Library for peeking and poking arbitrary memory locations.

- [Test2::Tools::FFI](https://metacpan.org/pod/Test2::Tools::FFI)

    Testing tools for FFI.

The latest versions as of when this [Task](https://metacpan.org/pod/Task) was released should be installed at minimum, if they are
not already installed.

Other prereqs may be added in the future if they are deemed useful for FFI development.

# CAVEATS

This module does require Perl 5.20 or better currently, because at least some of its prereqs require
that version.  Note that FFI bindings authored with these tools should work on Perls of at least
5.8.4 or better, so this is just a _development_ requirement.

This [Task](https://metacpan.org/pod/Task) indirectly requires [Alien::FFI](https://metacpan.org/pod/Alien::FFI).  If you do not want to build that from source
or do not have internet access where the build is happening, you will want to pre-install libffi.
On Debian based systems you can do that with `sudo apt-get update && sudo apt-get install libffi-dev`.

# AUTHOR

Graham Ollis <plicease@cpan.org>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2021 by Graham Ollis.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
