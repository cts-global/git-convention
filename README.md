# GIT CONVENTION
![git-workflow-release-cycle-4maintenance](https://github.com/cts-global/git-convention/assets/125328136/1d839d57-d503-4361-9849-51b70e234a74)


## <a id="Branch Naming Convention" href="'#Branch Naming Convention'">1. Branch Naming Convention</a>
Name branches according to the following convention:
### 1.1 Types
* A git branch should start with a category. Pick one of these: feature, bugfix, hotfix, or test.

    * `feature` is for adding, refactoring or removing a feature
    * `bugfix` is for fixing a bug
    * `hotfix` is for changing code with a temporary solution and/or without following the usual process (usually because of an emergency)
    * `test` is for experimenting outside of an issue/ticket

### 1.2 Reference
* After the category, there should be a "/" followed by the reference of the issue/ticket you are working on. 
* If there's no reference, just don't add.

### 1.3 Description
* After the reference, there should be another "/" followed by a description which sums up the purpose of this specific branch. This description should be short and "kebab-cased".
* By default, you can use the title of the issue/ticket you are working on. Just replace any special character by "-".

> [!IMPORTANT]
> Git branch follow below pattern:
> ### ``` git branch <category/[reference]/description-in-kebab-case> ``` 


### 1.4 Example 
```
  git branch feature/issue-42/create-new-button-component
```
```
  git branch feature/create-new-button-component
```
```
  git branch bugfix/issue-342/button-overlap-form-on-mobile
```


## <a id="Commit Naming Convention" href="'#Commit Naming Convention'">2. Commit Naming Convention</a>
### 2.1 Category 
* A commit message should start with a category of change. You can pretty much use the following 4 categories for everything: `feat`, `fix`, `refactor`, and `chore`.

  * ```feat``` is for adding a new feature
  * ```fix``` is for fixing a bug
  * ```refactor``` is for changing code for peformance or convenience purpose (e.g. readibility)
  * ```chore``` is for everything else (writing documentation, formatting, adding tests, cleaning useless code etc.)

* After the category, there should be a ":" announcing the commit description.

### 2.2 Statement
* After the colon, the commit description should consist in short statements describing the changes.
* Each statement should start with a verb conjugated in an imperative way.
* One commit should describe one task.

> [!IMPORTANT]
> Follow this pattern when committing:
> ### ```git commit -m '<category: do something>'```


### 2.4 Example 
```
  git commit -m 'feat: add new button component'
```
```
  git commit -m 'fix: add the stop directive to button component to prevent propagation'
```
```
  git commit -m 'refactor: rewrite button component in TypeScript'
```
```
  git commit -m 'chore: write button documentation'
```

## <a id="Some rules need to be followed" href="'#Some rules need to be followed'">3. Some rules need to be followed</a>
> [!IMPORTANT]
> * **Don't push directly to ```master```, ```main```, ```develop``` branches.**
> * **Format code before committing.**
> * **Avoid using ```git push -f``` or ```git push force```.**

## <a id="Reference" href="'#Some rules need to be followed'">4. Reference</a>
* [A Simplified Convention for Naming Branches and Commits in Git](https://dev.to/varbsan/a-simplified-convention-for-naming-branches-and-commits-in-git-il4)
* [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
