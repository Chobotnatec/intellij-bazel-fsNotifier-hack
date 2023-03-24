# IntelliJ fsNotifier fix for bazel codebases

fsNotifier chokes on some bazel codebases due to the large number of files and simlinks in the bazel folders.
My hacky fix is to ignore paths that has prefix `.bazel` and `bazel-` 

Use like this:
```bash
./make.sh
sudo mv fsnotifier <IDE_LOCATION>/bin/fsnotifier
```
