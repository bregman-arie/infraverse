In Jenkins, nodes are called "slaves" you connect between a node and a pipeline, in one of two ways, depends on the type of the pipeline.

### Declarative Pipeline

If a node has a label called "virtual":

```
pipelines {
    agent {label 'virtual'}
    stages {...}
    }
|
```

### Scripted Pipeline

If the node is called "some_node":

```
node ("some_node") {
    ...
}
```

If a node has a label called "virtual":

```
node (label: 'virtual') {
   ...
}
```
