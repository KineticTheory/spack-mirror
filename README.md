# Spack mirror for selected sources

## Adding more sources

```shell
$ git clone git@github.com:KineticTheory/spack-mirror
$ spack mirror create -d spack-mirror <spec>
$ cd spack-mirror
$ cd metis
$ spec=$(\ls)
$ loc=$(\ls -l $spec | sed -e 's/.*[ ]//')
$ rm $spec && mv $loc $spec
$ cd ..
$ git commit -a -m "Adding $spec" && git push
```
