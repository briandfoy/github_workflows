# Changes

These are the changes for [brian's Perl module GitHub workflows](https://github.com/briandfoy/github_actions).

## 20220125.002

* other workflows don't trigger on a release branch
* in the release workflow, do not trigger on the master branch. This leads to a [bad tag refs/head/master](https://github.com/actions/create-release/issues/13) as well as duplicate artifacts.

## 20220125.001

* adding a release workflow
