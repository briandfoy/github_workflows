 # brian's GitHub Actions

My personal [GitHub Actions](https://github.com/features/actions) for testing Perl modules. These files go in _.github/workflows/_ in each repo. Everything is available under the [Artistic 2.0 License](LICENSE)

* [macOS](perl-module-macos.yml)
* [Ubuntu](perl-module-ubuntu.yml)
* [Windows](perl-module-windows.yml)

## Some other demonstrations

I can trigger or ignore workflows or individual jobs. I'm mostly interested in switching on:

* branch name
* commit message

### Paying attention to things

A workflow or a job can run when a

* [workflow runs only if a branch matches](branches-macos.yml)

### Ignoring things

Sometimes I have a problem with one platform or part of the system. I
want to run some actions but not others. Instead of queueing all these builds and hoping the one I want runs soon, I just ignore a lot of them.

* [workflow ignores certain branches](.github/workflows/branches-ignore-macos-ubuntu.yml)
* [jobs ignore certain branches](.github/workflows/check-branch.yml)
* [check for flags in the commit message](.github/workflows/check-commit-message.yml)


## See Also

* [perl-github-actions-sample](https://github.com/skaji/perl-github-actions-sample)
* [Perl meets GitHub Actions](https://medium.com/@skaji/perl-meets-github-actions-3893ae100205)
* [GitHub Action for Perl Critic](https://github.com/marketplace/actions/github-action-for-perl-critic)
* [First steps with Github workflows](https://www.claudiokuenzler.com/blog/913/first-steps-github-actions-code-syntax-validation)
* [Setup Perl environment](https://github.com/marketplace/actions/setup-perl-environment)

## You might also like

* [brian's Standard Configuration for Perl 5 Modules on AppVeyor](https://github.com/briandfoy/brians_perl_modules_appveyor_config)
* [brian's Standard Configuration for Perl 5 Modules on Travis CI](https://github.com/briandfoy/brians_perl_modules_travis_config)
