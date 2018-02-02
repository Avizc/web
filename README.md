# Tiramisu

This is Avi's fork of the [pi-hole/web](https://github.com/pi-hole/web) project, a [ReactJS](https://reactjs.org/) based web interface for the [Pi-hole](https://github.com/pi-hole/pi-hole) project.

Why the fork?
-----------------
There are a few additions I'll be working on that would diverge too much most likely. Due to that this repo has been set up with a specific branching setup so I can work on my own additions and still pull down the original project and hopefully contribute to it, too!

Branching setup and naming scheme
-----------------
```
master ────────────────── sugar
├── coffee-production     ├── sugar-production
│   ├── coffee-dev        │   ├── sugar-dev
│   │   ├── try/example
```

* ```master``` - Incompatible changes with the original project, merge in ```sugar``` to stay current
* ```sugar``` - Perfect copy of the original project, merge in [upstream repo](https://github.com/pi-hole/web) to stay current
* ```coffee-production``` - Production branch, last checks and balances before merging to master
* ```coffee-dev``` - Merge in all dev branches, eventually merge to coffee-production
* ```sugar-production``` - Production branch for contributing, use this branch for submitting PRs to the [original project](https://github.com/pi-hole/web)
* ```sugar-dev``` - Merge in all dev branches for contributing to the original project, eventually merge to ```sugar-production```

Development branches take the following naming conventions:

* create - New features
* update - Updating existing features
* try - General branch for trying out new features, updates, fixes
* fix - Use for fixing bugs, errors, issues