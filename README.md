# IntelliJ fsNotifier fix for bazel codebases

fsNotifier chokes on some bazel code bases due to the large number of files in the bazel folders
My hacky fix is to ignore paths that contains `.bazel`

Use like this:
```bash
./make.sh
sudo mv fsnotifier64 /opt/JetBrains/idea-IU-211.7142.45/bin/fsnotifier64
```
