# Context

Facilitating easy service deployment and management.

Requirements:
- it needs to be possible to express & efficiently configure platform wide concernes
- it needs to be possible to express & efficiently configure project and service specific concernes
- As far as possible a platform maintainer should not need to understand the details of every particular project
- As far as possible an individual developer should only need to be concered with the specifics of their project or task

Solution:

Helm library charts that:
-  enable project, platform and subsystem wide configuration scopes.
-  provide resource definitions expressing "normal" service types in a manner that allows easy specialisation in the context of a single project.

fluxcd used to establish project tenants and deploy from git for dev/stage/prod. Initialy everything is dev.

skaffold via helm for developer deploys

render helm to git for fluxcd deploy. ultimately automated via branch an github actions
