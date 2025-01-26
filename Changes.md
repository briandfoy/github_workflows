# Changes

These are the changes for [brian's Perl module GitHub workflows](https://github.com/briandfoy/github_actions).

## 20250116.001

* Windows doesn't like cpanm installing App::Cpan because it thinks
the files are busy. So, just don't do that.

## 20250125.002

* Add environment variables EXTRA_CPANM_MODULES, with platform-specific versions `MACOS_*`, `UBUNTU_*`, and `WINDOWS_*`, which allows use to do things to install DBD::mysql@4.053 when
needed.

## 20250101.001

* Ignore `SECURITY.md` and `README.md` in linux, macos, and windows workflows

## 20220125.002

* other workflows don't trigger on a release branch
* in the release workflow, do not trigger on the master branch. This leads to a [bad tag refs/head/master](https://github.com/actions/create-release/issues/13) as well as duplicate artifacts.

## 20220125.001

* adding a release workflow
