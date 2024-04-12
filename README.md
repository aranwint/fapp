# Flutter application

This repo contains a simple Flutter project for my hometask. 


## Details

- The Flutter application inside of the repo is created by Android Studio by default. 
- This app is ready for building for iOS platforms by default. 
- Swift is chosen as iOS language for this project.


## How to run this GitHub action pipeline

Just push any commit to master branch and wait for the released package ;)

### Good to know

- The process of building and publishing you can watch in ['Flutter/Swift iOS app: build and publish' workflow](https://github.com/aranwint/fapp/actions/workflows/github-actions.yaml) section.
- All the releases are collected in [Releases](https://github.com/aranwint/fapp/releases) or [Tags](https://github.com/aranwint/fapp/tags) sections. Look at "Assets", here are link for downloading the released packages.


## Releasing

- A new release version and a tag on master-branch for releasing are being created automatically. 
- Any changes in master branch will be interpreted as a new release.
- Release number is based on current date and a unique GitHub Actions Run number for each run of a particular workflow in a repository. 
Every iteration this Run number will be increased by 1.
- Release version number is based on combination of a current date and GitHub Actions Run number (example v24.04.12.36)
- Restarting of the build in GitHub Actions Run will not be increase the release version.


## Artifacts

Github Actions build only xcarchive not-signed artifact and deploy releases in this GitHub repo.

[!] The dev-signature by Apple certificate is needed for next validation and distribution of the application.
Currently, this procedure has been delegated to the client's side.
xcarchive packages are ready for the signing in Xcode by an owner Apple Developer account.


## Write-up

The link to write-up file is provided with the link to this repository.

