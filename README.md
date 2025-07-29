# README

To test:
1. Make a change in any of the packages
2. Create PR
3. Change PR title to follow conventional commit -> PR check should pass
4. Merge PR
5. Check Actions tab for Release
6. New version should be published in EACH CHANGED packages

> [!NOTE]
> semantic-release is designed for 1 repo. semantic-release-monorepo extends it for monorepo, but it's unmaintained and does not include “dependency awareness”. 
> i.e. if  A depends on B, and B is changed, A won’t be updated (unless it has changes too)