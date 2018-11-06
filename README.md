# Test repo for version rolls

FVT is a test version of our main repo for practising version rolls and for
testing whether revving the `M` component in our `M.m.p` semantic versioning
scheme causes any issues in tooling or package dependencies.

## WARNING

DO NOT add this as another remote on your existing Flutter repo, particularly
if you're a Flutter committer. First, there's the risk of accidentally pushing
the fake version tags to the real upstream. Second this repo includes a
commit to README.md that is not checked into the real Flutter repo, so you're
risking future merge conflicts.

This repo is also significantly out-of-date when compared to the real repo.

## How to test

1. Clone this repo
2. Update your `PATH` environment variable to get rid of `flutter/bin` and add `fvt/bin`
3. Switch to stable channel: `flutter channel stable`
4. Run flutter upgrade: `flutter upgrade`
5. Test away! Run the gallery, test against your own apps, build a codelab.
