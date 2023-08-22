# Server Configs

Requires Ubuntu OpenJDK or [Microsoft OpenJDK 17](https://www.microsoft.com/openjdk)

Start with

```bash
java -Xms2000M -Xmx8000M "-Dterminal.ansi=true" "-XX:+UnlockExperimentalVMOptions" "-XX:+UnlockDiagnosticVMOptions" "-XX:AllocatePrefetchStyle=3" "-XX:+AlwaysPreTouch" "-XX:+DisableExplicitGC" "-XX:-DontCompileHugeMethods" "-XX:G1ConcMarkStepDurationMillis=5" "-XX:G1ConcRefinementServiceIntervalMillis=150" "-XX:G1ConcRSHotCardLimit=16" "-XX:G1HeapRegionSize=16M" "-XX:G1MixedGCCountTarget=3" "-XX:G1MixedGCLiveThresholdPercent=90" "-XX:G1NewSizePercent=28" "-XX:G1ReservePercent=20" "-XX:G1RSetUpdatingPauseTimePercent=0" "-XX:G1SATBBufferEnqueueingThresholdPercent=30" "-XX:InitiatingHeapOccupancyPercent=10" "-XX:MaxGCPauseMillis=130" "-XX:MaxNodeLimit=240000" "-XX:MaxTenuringThreshold=1" "-XX:NmethodSweepActivity=1" "-XX:NodeLimitFudgeFactor=8000" "-XX:NonNMethodCodeHeapSize=12M" "-XX:NonProfiledCodeHeapSize=194M" "-XX:+PerfDisableSharedMem" "-XX:ProfiledCodeHeapSize=194M" "-XX:ReservedCodeCacheSize=400M" "-XX:SurvivorRatio=32" "-XX:ThreadPriorityPolicy=1" "-XX:+UseCriticalJavaThreadPriority" "-XX:+UseFastUnorderedTimeStamps" "-XX:+UseNUMA" "-XX:+UseVectorCmov" "-Dusing.aikars.flags=https://mcflags.emc.gs" "-Daikars.new.flags=true" "-Ddisable.book-limits=true" -jar server.jar
```
