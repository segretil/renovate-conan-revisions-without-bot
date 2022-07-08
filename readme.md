# Renovate-conan-revisions 

### Context
Renovate does not update the conan revisions.

For more details go see: https://github.com/renovatebot/renovate/issues/16467

### What happened 
Renovate created two merge requests: 
- [For glm](https://github.com/segretil/renovate-conan-revisions/pull/3)
- [For cairo](https://github.com/segretil/renovate-conan-revisions/pull/2)

The glm pull request works, but the cairo one is going to trigger a conan error because the revision is incorrect.

### What I expect
I expect three pull requests here:
- For glm
- For cairo 
- For opus 

The glm one is already correct. 

For cairo I expect this: 
```diff
- cairo/1.17.2@_/_#aff2d03608351db075ec1348a3afc9ff
+ cairo/1.17.4@_/_#51627b399b12479e23cc7958a33fb5eb
```

For opus I expect this:
```diff
- opus/1.3.1@_/_#6d2446ed5a38e86a3bb304db3ffb3e01
+ opus/1.3.1@_/_#5132ab8db7b69dd8e26466e0b3b017dd
```
