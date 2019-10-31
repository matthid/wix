
# Wix 3

1. choco install html-help-workshop
2. a) Install C++ Visual Studio Desktop Development Workload: https://stackoverflow.com/questions/42701019/problems-generating-solution-for-vs-2017-with-cmake
2. b) Install v141 tools
      > `error MSB8020: The build tools for v141_xp (Platform Toolset = 'v141_xp') cannot be found`
3. Edit WixBuild.props (update Win10 SDK path if required)
   > `'"\bin\rc.exe"' is not recognized as an internal or external command,`
4. msbuild tools\OneTimeWixBuildInitialization.proj
5. msbuild wix.proj