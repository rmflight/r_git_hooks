# R Package Git Commit Hooks

These are a pre-commit and post-commit hooks that checks that there are 
files to be committed, and if there are, increments the package version in the 
DESCRIPTION file, either before or after the actual commit.

The pre-commit hook also checks if the version in the DESCRIPTION has any manual changes, and
doesn't increment if there are any there.

## License

CC0

## Installation 

Copy the contents of the hook you want to use to

```
package_directory/.git/hooks/pre-commit

or

package_directory/.git/hooks/post-commit
```

and make it executable. Make sure that Rscript is on your path.
