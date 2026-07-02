<!--

    Copyright (c) 2011-present Sonatype, Inc. All rights reserved.
    Includes the third-party code listed at http://links.sonatype.com/products/clm/attributions.
    "Sonatype" is a trademark of Sonatype, Inc.

-->
## Description

Please include a summary of the change.

Example:  This change will update the existing kubecost configuration and add a new ingress path.

## Potential Impact

Please describe the reason and potential impact on the business and security environment.

## Jira

Please include a link to the Jira.

Example: https://sonatype.atlassian.net/browse/SRE-1739

## Type of change

Please delete the option that is not relevant.

- [x] Bug fix (non-breaking change which fixes an identified issue)
- [x] New feature (non-breaking change which adds functionality)
- [x] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [x] Documentation - No new functionality added to codebase

## How Has This Been Tested?

Please describe the tests that you ran to verify your changes.

Example: I have run the tests against the pre-provisioned ephemeral cluster sre-sre-1739-cmcf-eks-cluster.  The cluster is still available.

## Documentation

Provide a link to the documentation. 
If this is a large change please fill out the following checklist:
- [ ] I have included system description and purpose to the docs.
- [ ] I have included information involved with classification.
- [ ] I have included data flow and architecture diagrams.
- [ ] I have included primary roles for key users of the system.

Example for external source: https://docs.sonatype.com/pages/viewpage.action?spaceKey=SRE&title=Cloudy+McCloudface
Example for internal source: docs/runbook/RUNBOOK.md

## License Check


Please ensure you run the license check.  You can run the license check from the base of this repository:

```
docker run --rm -v $(pwd):/license-check/src docker-all.repo.sonatype.com/cdi/license-check:latest -f
```

## Checklist:

- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have added the Jira link
- [ ] I have added tests that proves my code works, if applicable
- [ ] I have run the license check, if applicable
- [ ] I have included documentation!