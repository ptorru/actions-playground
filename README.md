# Releases
GitHub can show releases of your repo. It does this by using tags as means to select a version of the code for a given release.

Ideally you want all the admin related to your releases to be done automatically, eg, for every new release tag created:
* Build all artifacts.
* Create the release.
* Upload the artifacts to the release.

## Using Tags
Ideally you want to have a `github-release` created when you create a release tag, together with the artifacts uploaded to it.

This behaviour is implemented by [upload-release-action](https://github.com/svenstaro/upload-release-action)

Inspiration on how to do this without limiting the use of tags for other things came from [nwillc](https://github.community/t/merge-matrix-build-artifacts-for-release/118190)
