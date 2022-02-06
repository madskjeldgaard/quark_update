# Quark update script

*Update a SuperCollider quark's version, set the git tag and auto generate a changelog in one go.*

This is a simple script that takes care of a few of the important steps in updating a SuperCollider quark's version number. I keep forgetting the steps necessary and even more often I forget the sequence of those steps, so this script just makes it easy.

It uses [git-cliff](https://github.com/orhun/git-cliff) and assumes you have that installed. It also assumes you use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)..

An example of this script used in the wild [is here](https://codeberg.org/madskjeldgaard/mk-synthlib/src/branch/main/CHANGELOG.md).

## Usage

Open a terminal in the root of your quark's folder.

If you don't have a cliff config, run `git  cliff --init` to generate the .toml format config file it uses. This is specific to your quark.

Then, from the root of your quark's folder, run `quark_update 0.5` to update your quark to version 0.5.
