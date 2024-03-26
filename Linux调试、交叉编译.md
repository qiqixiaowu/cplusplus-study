1. 调试选项连接linux机器
2. Cmakelist.txt 与 CmakeSettings.json
  CmakeSettings提供了一种灵活且可定制化的方式来配置CMake项目，使得项目的构建更加方便和高效
eg:
{
  "configurations": [
    {
      "buildCommandArgs": "",
      "cmakeCommandArgs": "",
      "configurationType": "Release",
      "ctestCommandArgs": "",
      "generator": "Unix Makefiles",
      "inheritEnvironments": [ "linux_x64" ],
      "name": "Linux-GCC-Release",
      "remoteBuildRoot": "$HOME/test/uhive-appcomponent/out",
      "remoteCMakeListsRoot": "$HOME/test/uhive-appcomponent",
      "remoteCopyBuildOutput": false,
      "remoteCopySources": true,
      "remoteCopySourcesExclusionList": [ ".vs", ".git", "out" ],
      "remoteCopySourcesMethod": "rsync",
      "remoteInstallRoot": "$HOME/ShenZhou/server/UIH",
      "remoteMachineName": "${defaultRemoteMachineName}",
      "rsyncCommandArgs": "-t --delete --delete-excluded",
      "cmakeExecutable": "cmake"
    }
  ]
}
3. 
