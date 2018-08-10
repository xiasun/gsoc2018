---
layout: default
---
### Introduction

This is the introduction of surface reconstruction tool of 3DTK.

### Sample usages

1. Use the default sample data under `dat/` directory, with all scans join first, poisson octree depth 12 and trimming value 7.0.
```shell
bin/recon dat dat/test/xiaosaomao -t true -d 12 -T 7.0 -j true
```
![dat](imgs/model_all_trimmed.png)
---
2. Use a common points data, for example the [Stanford Bunny](http://graphics.stanford.edu/data/3Dscanrep/#bunny). A recommended way is convert the original model file into .xyz file that only contains the xyz coordinates, rename it as `scan000.3d` and put it into a directory for example `dat/bunny/`, new a file called `scan000.pose` and put it under the same directory, and then use commands below.
```shell
bin/recon dat/bunny dat/bunny/model --inward false
```
![bunny](imgs/bunny.png)

---

### Options list
##### Mandatory options
##### I/O options
##### Normal calculation options
##### Scan joining options
##### Poisson options

### Commits



