Hi!  This is my personal website, with thoughts & semi-broken projects and the like.

Visit it here [https://programmatix.github.io/Words/projects/](https://programmatix.github.io/Words/projects/).

## Initial
Install Hugo from https://gohugo.io/
```
cd themes
git clone https://github.com/spf13/hyde.git
cd ..
hugo
```

## Developing
```
hugo server -D
```

Open http://localhost:1313/Words/

## Release Process
```
hugo
git add docs
git commit -a -m "Commit message"
git push
```

## Dev notes
hugo is setup to create the site in the docs directory, and Git Pages serves from this folder.
