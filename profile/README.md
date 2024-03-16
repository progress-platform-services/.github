# Progress Platform Services
This organization holds applications, components and user experiences architected as a single Progress platform to build multiple applications in the infrastructure business unit.  These "building blocks" and finished applications can be reused across teams to reduce duplication of effort and promote common practice especially for "plumbing" areas which do not provide good business value.  

## Contributing
Inner-sourced, collaborative requirements gathering

Each team can select its own programming language, storage and DevOps scripting languages, as well as the distribution targets for their applications (e.g., Darwin/ARM, RHEL 7 or 9, etc.).  

Two general purpose standards apply:
- OpenAPI version 3.0
- Open container initiative 

## Licensing
All repositories in this organization are "internal" which means they are shared with all Progress employees with access to the organization.  Ideally this is broad, cross-business unit participation so that components can be developed and shared broadly.  These repositories should not be marked "private" since that incurs a burden on maintaining specific user access lists.  A maintainer group can be created to know where feedback and bugs should be reported.

Internal repositories do not need a LICENSE.txt and are assumed to be proprietary property of Progress.  That is, copyright based on the year of initial development with all rights reserved.  If a repository is to be made open source or have a specific license applied for source code sharing (typically Progress uses Apache v2.0 - https://www.apache.org/licenses/LICENSE-2.0.txt), please prepare to move the code to another organization like inspec and consult your legal support for markings.

## Common CI/CD build pipelines
Each repository will use GitHub Actions to perform continuous integration (CI) tasks -- creating a binary, unit testing, static security checks, building bills of material (SBOM), etc. -- and some repositories may include continuous deployment of applcations to hosted environments.

Artifacts and binaries will be on the Releases tab for a given module or application repository. 

## Specific repositories of interest
- **code-gen** provides a GoLang-based code scaffold for REST-based API services
- **open-api-specifications** a repository of Chef Courier APIs used to generate browsable documentation
- **helm** CD scripts to deploy services for Chef Courier and other products
- **.github** provides common GitHib Actions for CI and CD, for API services, command-line interfaces (CLI), Courier Agents, and jobs.
- **scripts** provide general purpose bash/sh and PowerShell scripts for common repository operations

## References
1. https://docs.github.com/en/actions/using-workflows/creating-starter-workflows-for-your-organization
1. https://en.wikipedia.org/wiki/Inner_source
1. https://about.gitlab.com/topics/version-control/what-is-innersource/
1. https://resources.github.com/innersource/fundamentals/
1. https://www.gnu.org/philosophy/philosophy.html