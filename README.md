# be-infrastructure-networking

Build AWS networking components that can be reused by other projects.

## Infrastructure

This service consists of the following stack(s):

- `00-pipeline.yml` - stack deploying the aws codepipeline which in turn will deploy the other stacks
- `01-infrastructure` - stack deploying the aws networking components

## Depedencies

None.

## Deployment

This project is deployed via AWS Code pipeline.

A github webhook has been configured so that any push to the repo will trigger the pipeline.

## Monitoring

None.

## Tests

None.

---

## Notes

None.

## Todo list

* Pipeline.yml
  - Create a machine user to limit access to github
  - webhook: secure webhook from [github](https://developer.github.com/webhooks/securing/)
