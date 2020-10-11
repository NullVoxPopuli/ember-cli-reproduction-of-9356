Reproduction steps:

While in the root directory:

1. `ember addon my-addon --yarn --skip-git`
2. `ember new my-app --yarn --skip-git`
3. `( cd my-addon && ember g template application )`
4. `( cd my-addon && yarn )`
5. Add `"my-addon": "link:../my-addon",` to the app's package.json
6. `( cd my-app && yarn && ember build  )`


