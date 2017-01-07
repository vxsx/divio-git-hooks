# Divio Git Hooks

This repo contains git hooks which I find useful when working on [Divio Clould](http://divio.com) projects.

## post-merge

* If after pulling the python or node requirements changed - will ask if you want to rebuild the container immediately
* If after pulling any sass or js files changed - will rebuild static files (especially useful if you don't actively work on styles)

Install (run in root of the project): 

```
curl -o .git/hooks/post-merge -L https://raw.githubusercontent.com/vxsx/divio-git-hooks/master/post-merge && chmod +x .git/hooks/post-merge
```
