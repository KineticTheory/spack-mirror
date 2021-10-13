# Spack mirror for selected sources

## Adding more sources

```shell
$ git clone git@github.com:KineticTheory/spack-mirror
$ spack mirror create -d spack-mirror <spec>
$ cd spack-mirror && git commit -a -m "Adding <spec>" && git push
```
