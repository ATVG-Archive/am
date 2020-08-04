# AM - Automated Make build system

This is the AM - Automated Make Build System. This script automates the usage of Makefile, Ninja and CMake into a way it is simple to use.

**This Script does not replace Make, CMake or Ninja. It only automates them based on what files exit!**

This script could be improved more, but it works. And this is how:

```
* Clone Git repo (if -c http://your-remote.com/project.git given)
  * Clone into -td /path
  * Move to -td if given
* Check for build/
  * Build exists, Check for build.old/
    * Build.old exists, delete
  * Move build to build.old
* Create build/
* Check for Git (if not --no-git-modules)
  * No Git, exit
  * Check for .gitmodules
    * No modules, exit
  * Run submodule init
  * Run submodule update
* Check for Cmake
  * No Cmake, Check for Make
    * No Make, Check for Ninja
      * No Ninja, exit
    * Check that Ninja is installed
    * Run Ninja
  * Check that Make is installed
  * Run Make
* Check that CMake is installed
* Run CMake
  * Check for Make
    * No Make, Check for Ninja
      * No Ninja, exit
    * Check that Ninja is installed
    * Run Ninja
  * Check that Make is installed
  * Run Make
* If $1 was -l, print log (build/am-build.log)
* Exit
```

# License

This project is licensed under the [OSPL20](/LICENSE).
