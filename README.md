#### Rebuilding the `Packages` file

With your updated `control` file, build your tweak.
Store the resulting `.deb.` file into the `/debs/` folder of your repo.
Build your `Packages` file and compress with `bzip2`.

cd /Users/michaelmelita/michaelmelita1.github.io-master

dpkg-scanpackages -m ./debs > Packages

bzip2 Packages
```
