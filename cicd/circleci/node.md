In CircleCI, the hosts/executors on which a pipeline is executed, is called a runner.<br>
You reference a runner on a job in the file `.circleci/config.yml` like this:

```
version: 2.1
workflows:
  testing:
    jobs:
      - runner
jobs:
  runner:
    machine: true
    resource_class: your-namespace/your-resource
    steps:
      - run: echo "Hi I'm on Runners!"
```

The above example is taken from [CircleCI docs](https://circleci.com/docs/2.0/runner-overview/?section=executors-and-images)
