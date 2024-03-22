# Common GitHub Actions
For CI and CD

## CI
Top level naming starts with type (**ci** or **cd**), then application style
- cli
- service
- agent
- job

Followed by language (**go**)

Followed by applicable branch
- main
- develop
- release
- multiple

If there is no extension then it is the actual workflow.  If the extension **-dispatch** is present, then this workflow can be run from the GitHub repositiory action page (allows entry of variables).  If the extension **-stub** is present, this is the reference workflow to go into a repository's .github/workflows directory (code generation will put this in a repo).

Artifacts and binaries will be on the Releases tab for a given module or application repository. 

## list (remove when done)
- ci-cli-go-main
- ci-cli-go-main-dispatch
- ci-cli-go-main-stub

- ci-helm-publish - needs checkov
- cd-helm-eks-chef-platform-dev

- ci-service-go-main
- ci-service-go-main-dispatch
- ci-service-go-main-stub
- ci-service-go-main
- Powershell to delete junk PR-builds

- ci-userinterface-angular-main
