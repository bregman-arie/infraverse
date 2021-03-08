In Gitlab nodes on which pipelines are executed, are called "Runners".

There are shared runners and specific runners. When setting up a shared runner, your pipeline will automatically use that pipeline by default.<br>
In order to limit a pipeline to a specific runner, you need to use tags. This is how it looks:

```
job:
  tags:
    - docker
```

The pipeline will run only on runners tagged with `docker`.
