# Dockerfile for hg-fast-export tool

Dockerfile for [https://github.com/frej/fast-export](https://github.com/frej/fast-export)

## Usage

1. Create a target directory and initialise an empty git repository in it (using `git init`)
1. Convert a mercurial repository to the git repository with the following command:

        docker run --rm -v <src>:/hg -v <dst>:/git zerkms/hg-fast-export

    Where `<src>` and `<dst>` are the full paths to the source and destination repositories correspondingly.
