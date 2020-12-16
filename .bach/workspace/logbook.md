# Logbook of mainrunner 2.2-ea+ebe4c24

- Created at 2020-12-16 08:13:17.842
- Written at 2020-12-16 08:13:24.836

## Modules

- directory: file:///home/runner/work/mainrunner/mainrunner/.bach/workspace/modules/
- files: 2

### Module API

| Name | Version | Exports | Provides | Main Class |
|------|---------|---------|----------|------------|
|`com.github.sormuras.mainrunner.api`|2.2-ea+ebe4c24|`com.github.sormuras.mainrunner.api`|`-`|`-`|
|`com.github.sormuras.mainrunner.engine`|2.2-ea+ebe4c24|`-`|`org.junit.platform.engine.TestEngine with [com.github.sormuras.mainrunner.engine.Mainrunner]`|`-`|

### Modular JAR

| Size [Bytes] | File Name |
|-------------:|:----------|
|2,768|com.github.sormuras.mainrunner.api@early-access.jar
|14,341|com.github.sormuras.mainrunner.engine@early-access.jar

## Project

- name: mainrunner
- version: 2.2-ea+ebe4c24

### Project Descriptor

```text
Project
  name: mainrunner
  version: 2.2-ea+ebe4c24
  externals: ExternalModules
      requires: [org.assertj.core, org.junit.jupiter, org.junit.platform.console, org.junit.platform.engine, org.junit.platform.launcher, org.junit.platform.testkit]
      links: []
      lookups: []
  spaces: CodeSpaces
      main: MainCodeSpace
          modules: ModuleDeclarations
              map: (KEY) -> VALUE
              (com.github.sormuras.mainrunner.api) -> ModuleDeclaration
                  reference: ModuleInfoReference[info=com.github.sormuras.mainrunner.api/main/java-module/module-info.java]
                  sources: SourceFolders
                      list: [SourceFolder[path=com.github.sormuras.mainrunner.api/main/java, release=0], SourceFolder[path=com.github.sormuras.mainrunner.api/main/java-module, release=0]]
                  resources: SourceFolders
                      list: []
              (com.github.sormuras.mainrunner.engine) -> ModuleDeclaration
                  reference: ModuleInfoReference[info=com.github.sormuras.mainrunner.engine/main/java-module/module-info.java]
                  sources: SourceFolders
                      list: [SourceFolder[path=com.github.sormuras.mainrunner.engine/main/java, release=0], SourceFolder[path=com.github.sormuras.mainrunner.engine/main/java-eleven, release=0], SourceFolder[path=com.github.sormuras.mainrunner.engine/main/java-module, release=0]]
                  resources: SourceFolders
                      list: [SourceFolder[path=com.github.sormuras.mainrunner.engine/main/resources, release=0]]
          modulePaths: ModulePaths
              paths: [.bach/external-modules]
          release: 8
          jarslug: early-access
          launcher: Launcher
              name: mainrunner
              module: 
          features: Features
              set: [GENERATE_API_DOCUMENTATION]
          tweaks: Tweaks
              list: [Tweak[trigger=javadoc, arguments=[-encoding, UTF-8]], Tweak[trigger=javadoc, arguments=[-windowtitle, 🦄 Mainrunner]], Tweak[trigger=javadoc, arguments=[-header, 🦄 Mainrunner]], Tweak[trigger=javadoc, arguments=[-doctitle, 🦄 Mainrunner 2.2-ea]], Tweak[trigger=javadoc, arguments=[-overview, .bach/api-overview.html]], Tweak[trigger=javadoc, arguments=[-notimestamp]]]
      test: TestCodeSpace
          modules: ModuleDeclarations
              map: (KEY) -> VALUE
              (test.integration) -> ModuleDeclaration
                  reference: ModuleInfoReference[info=test.integration/test/java/module-info.java]
                  sources: SourceFolders
                      list: [SourceFolder[path=test.integration/test/java, release=0]]
                  resources: SourceFolders
                      list: []
              (test.programs) -> ModuleDeclaration
                  reference: ModuleInfoReference[info=test.programs/test/java/module-info.java]
                  sources: SourceFolders
                      list: [SourceFolder[path=test.programs/test/java, release=0]]
                  resources: SourceFolders
                      list: []
          modulePaths: ModulePaths
              paths: [.bach/workspace/modules, .bach/external-modules]
          tweaks: Tweaks
              list: [Tweak[trigger=javadoc, arguments=[-encoding, UTF-8]], Tweak[trigger=javadoc, arguments=[-windowtitle, 🦄 Mainrunner]], Tweak[trigger=javadoc, arguments=[-header, 🦄 Mainrunner]], Tweak[trigger=javadoc, arguments=[-doctitle, 🦄 Mainrunner 2.2-ea]], Tweak[trigger=javadoc, arguments=[-overview, .bach/api-overview.html]], Tweak[trigger=javadoc, arguments=[-notimestamp]]]
```

## Tool Call Overview

|    |Thread| Duration |Tool|Arguments
|----|-----:|---------:|----|---------
|    |     1|    0.808s|[javac](#javac-45e140ae)|`--release 16 --module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -d .bach/workspace/classes-main/16`
|    |     1|     0.13s|[javac](#javac-48cdb156)|`--release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.api/main/java-module/module-info.java`
|    |     1|    0.131s|[javac](#javac-4b4814d0)|`--release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Main.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/package-info.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/MainRepeatable.java`
|    |     1|    0.243s|[javac](#javac-4ae8fb2a)|`--release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.engine/main/java-module/module-info.java`
|    |     1|    0.436s|[javac](#javac-54326e9)|`--release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Overlay.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/OverlaySingleton.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/AbstractClassBasedTestEngine.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Mainrunner.java`
|    |     1|    0.019s|[jar](#jar-20216016)|`--create --file .bach/workspace/modules/com.github.sormuras.mainrunner.api@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api .`
|    |     1|    0.004s|[jar](#jar-2b441e56)|`--create --file .bach/workspace/modules/com.github.sormuras.mainrunner.engine@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine . -C com.github.sormuras.mainrunner.engine/main/resources .`
|    |     1|    1.394s|[javadoc](#javadoc-267891bf)|`--module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -encoding UTF-8 -windowtitle 🦄 Mainrunner -header 🦄 Mainrunner -doctitle 🦄 Mainrunner 2.2-ea -overview .bach/api-overview.html -notimestamp -d .bach/workspace/documentation/api`
|    |     1|    0.067s|[jar](#jar-3a109ff7)|`--create --file .bach/workspace/documentation/mainrunner-api-2.2-ea+ebe4c24.zip --no-manifest -C .bach/workspace/documentation/api .`
|    |     1|     0.22s|[javac](#javac-111a7973)|`--module test.integration,test.programs --module-source-path ./*/test/java --module-path .bach/workspace/modules:.bach/external-modules -d .bach/workspace/classes-test/16`
|    |     1|    0.024s|[jar](#jar-1a2773a8)|`--create --file .bach/workspace/modules-test/test.integration@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.integration .`
|    |     1|    0.077s|[jar](#jar-78b0ec3a)|`--create --file .bach/workspace/modules-test/test.programs@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.programs .`
|    |     1|    0.414s|[junit](#junit-46612bfc)|`--select-module test.integration --reports-dir .bach/workspace/reports/junit-test/test.integration`
|    |     1|    0.237s|[junit](#junit-4f213a2)|`--select-module test.programs --reports-dir .bach/workspace/reports/junit-test/test.programs`

## Tool Call Details

Recorded 14 tool call response(s).

### javac-45e140ae

- tool = `javac`
- args = `--release 16 --module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -d .bach/workspace/classes-main/16`

### javac-48cdb156

- tool = `javac`
- args = `--release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.api/main/java-module/module-info.java`

### javac-4b4814d0

- tool = `javac`
- args = `--release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Main.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/package-info.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/MainRepeatable.java`

### javac-4ae8fb2a

- tool = `javac`
- args = `--release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.engine/main/java-module/module-info.java`

### javac-54326e9

- tool = `javac`
- args = `--release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Overlay.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/OverlaySingleton.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/AbstractClassBasedTestEngine.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Mainrunner.java`

### jar-20216016

- tool = `jar`
- args = `--create --file .bach/workspace/modules/com.github.sormuras.mainrunner.api@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api .`

### jar-2b441e56

- tool = `jar`
- args = `--create --file .bach/workspace/modules/com.github.sormuras.mainrunner.engine@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine . -C com.github.sormuras.mainrunner.engine/main/resources .`

### javadoc-267891bf

- tool = `javadoc`
- args = `--module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -encoding UTF-8 -windowtitle 🦄 Mainrunner -header 🦄 Mainrunner -doctitle 🦄 Mainrunner 2.2-ea -overview .bach/api-overview.html -notimestamp -d .bach/workspace/documentation/api`

```text
Constructing Javadoc information...
Creating destination directory: ".bach/workspace/documentation/api/"
Building index for all the packages and classes...
Standard Doclet version 16-ea+28
Building tree for all the packages and classes...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/Java.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/Main.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/MainRepeatable.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/Java.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/Main.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/MainRepeatable.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/package-summary.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/com/github/sormuras/mainrunner/api/package-tree.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.api/module-summary.html...
Generating .bach/workspace/documentation/api/com.github.sormuras.mainrunner.engine/module-summary.html...
Generating .bach/workspace/documentation/api/overview-tree.html...
Generating .bach/workspace/documentation/api/index.html...
Building index for all classes...
Generating .bach/workspace/documentation/api/allclasses-index.html...
Generating .bach/workspace/documentation/api/allpackages-index.html...
Generating .bach/workspace/documentation/api/index-all.html...
Generating .bach/workspace/documentation/api/overview-summary.html...
Generating .bach/workspace/documentation/api/help-doc.html...
6 warnings
```

```text
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Main.java:12: warning: no comment
public @interface Main {
        ^
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java:10: warning: no comment
public @interface Java {
        ^
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/MainRepeatable.java:10: warning: no comment
public @interface MainRepeatable {
        ^
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java:12: warning: no comment
  String[] options() default {};
           ^
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java:14: warning: no comment
  int expectedExitValue() default 0;
      ^
./com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/MainRepeatable.java:11: warning: no comment
  Main[] value();
         ^
```

### jar-3a109ff7

- tool = `jar`
- args = `--create --file .bach/workspace/documentation/mainrunner-api-2.2-ea+ebe4c24.zip --no-manifest -C .bach/workspace/documentation/api .`

### javac-111a7973

- tool = `javac`
- args = `--module test.integration,test.programs --module-source-path ./*/test/java --module-path .bach/workspace/modules:.bach/external-modules -d .bach/workspace/classes-test/16`

```text
Note: ./test.integration/test/java/test/integration/IntegrationTests.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
```

### jar-1a2773a8

- tool = `jar`
- args = `--create --file .bach/workspace/modules-test/test.integration@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.integration .`

### jar-78b0ec3a

- tool = `jar`
- args = `--create --file .bach/workspace/modules-test/test.programs@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.programs .`

### junit-46612bfc

- tool = `junit`
- args = `--select-module test.integration --reports-dir .bach/workspace/reports/junit-test/test.integration`

```text
Thanks for using JUnit! Support its development at https://junit.org/sponsoring

╷
├─ JUnit Jupiter ✔
│  └─ IntegrationTests ✔
│     └─ verifyMainrunnerStatistics() ✔
└─ Mainrunner (Java 8) ✔
   └─ IntegrationTests ✔
      └─ main() ✔

Test run finished after 129 ms
[         4 containers found      ]
[         0 containers skipped    ]
[         4 containers started    ]
[         0 containers aborted    ]
[         4 containers successful ]
[         0 containers failed     ]
[         2 tests found           ]
[         0 tests skipped         ]
[         2 tests started         ]
[         0 tests aborted         ]
[         2 tests successful      ]
[         0 tests failed          ]
```

### junit-4f213a2

- tool = `junit`
- args = `--select-module test.programs --reports-dir .bach/workspace/reports/junit-test/test.programs`

```text
Thanks for using JUnit! Support its development at https://junit.org/sponsoring

╷
├─ JUnit Jupiter ✔
└─ Mainrunner (Java 8) ✔
   └─ TestProgram ✔
      └─ main() ✔

Test run finished after 36 ms
[         3 containers found      ]
[         0 containers skipped    ]
[         3 containers started    ]
[         0 containers aborted    ]
[         3 containers successful ]
[         0 containers failed     ]
[         1 tests found           ]
[         0 tests skipped         ]
[         1 tests started         ]
[         0 tests aborted         ]
[         1 tests successful      ]
[         0 tests failed          ]
```

## All Entries

```text
DEBUG        1| Execute default build program
DEBUG        1| Compile build module: javac --module build --module-source-path .bach --module-path .bach/cache -encoding UTF-8 -d .bach/workspace/.bach
DEBUG        1| project-info -> @com.github.sormuras.bach.project.ProjectInfo(lookups={}, tweaks={@com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-encoding", "UTF-8"}), @com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-windowtitle", "\ud83e\udd84 Mainrunner"}), @com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-header", "\ud83e\udd84 Mainrunner"}), @com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-doctitle", "\ud83e\udd84 Mainrunner 2.2-ea"}), @com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-overview", ".bach/api-overview.html"}), @com.github.sormuras.bach.project.ProjectInfo$Tweak(in={MAIN, TEST}, tool="javadoc", with={"-notimestamp"})}, version="2.2-ea", testModulePaths={".bach/workspace/modules", ".bach/external-modules"}, modules={"com.github.sormuras.mainrunner.api/main/java-module/module-info.java", "com.github.sormuras.mainrunner.engine/main/java-module/module-info.java"}, modulePaths={".bach/external-modules"}, launchCustomRuntimeImageWithModule="*", compileModulesForJavaRelease=8, features={GENERATE_API_DOCUMENTATION}, tests={"test.integration/test/java/module-info.java", "test.programs/test/java/module-info.java"}, name="*", links={}, requires={})
INFO         1| Build project mainrunner 2.2-ea+ebe4c24
DEBUG        1| Load required and missing modules
INFO         1| Compile 2 main modules
INFO         1| Run javac with 12 arguments
DEBUG        1| javac --release 16 --module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -d .bach/workspace/classes-main/16
INFO         1| Run javac with 12 arguments
DEBUG        1| javac --release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.api/main/java-module/module-info.java
INFO         1| Run javac with 10 arguments
DEBUG        1| javac --release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Main.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/Java.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/package-info.java com.github.sormuras.mainrunner.api/main/java/com/github/sormuras/mainrunner/api/MainRepeatable.java
INFO         1| Run javac with 12 arguments
DEBUG        1| javac --release 9 --module-version 2.2-ea+ebe4c24 --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -implicit:none -d .bach/workspace/classes-main/8 com.github.sormuras.mainrunner.engine/main/java-module/module-info.java
INFO         1| Run javac with 10 arguments
DEBUG        1| javac --release 8 --class-path .bach/workspace/classes-main/16/com.github.sormuras.mainrunner.api:.bach/workspace/classes-main/16/com.github.sormuras.mainrunner.engine:.bach/external-modules/org.apiguardian.api.jar:.bach/external-modules/org.assertj.core.jar:.bach/external-modules/org.junit.jupiter.api.jar:.bach/external-modules/org.junit.jupiter.engine.jar:.bach/external-modules/org.junit.jupiter.jar:.bach/external-modules/org.junit.jupiter.params.jar:.bach/external-modules/org.junit.platform.commons.jar:.bach/external-modules/org.junit.platform.console.jar:.bach/external-modules/org.junit.platform.engine.jar:.bach/external-modules/org.junit.platform.launcher.jar:.bach/external-modules/org.junit.platform.reporting.jar:.bach/external-modules/org.junit.platform.testkit.jar:.bach/external-modules/org.opentest4j.jar -d .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Overlay.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/OverlaySingleton.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/AbstractClassBasedTestEngine.java com.github.sormuras.mainrunner.engine/main/java/com/github/sormuras/mainrunner/engine/Mainrunner.java
INFO         1| jar(com.github.sormuras.mainrunner.api)
DEBUG        1| jar --create --file .bach/workspace/modules/com.github.sormuras.mainrunner.api@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.api .
INFO         1| jar(com.github.sormuras.mainrunner.engine)
DEBUG        1| jar --create --file .bach/workspace/modules/com.github.sormuras.mainrunner.engine@early-access.jar -C .bach/workspace/classes-main/8/com.github.sormuras.mainrunner.engine . -C com.github.sormuras.mainrunner.engine/main/resources .
INFO         1| Generate API documentation
INFO         1| Run javadoc with 19 arguments
DEBUG        1| javadoc --module com.github.sormuras.mainrunner.api,com.github.sormuras.mainrunner.engine --module-source-path ./*/main/java:./*/main/java-module --module-path .bach/external-modules -encoding UTF-8 -windowtitle 🦄 Mainrunner -header 🦄 Mainrunner -doctitle 🦄 Mainrunner 2.2-ea -overview .bach/api-overview.html -notimestamp -d .bach/workspace/documentation/api
INFO         1| Run jar with 7 arguments
DEBUG        1| jar --create --file .bach/workspace/documentation/mainrunner-api-2.2-ea+ebe4c24.zip --no-manifest -C .bach/workspace/documentation/api .
INFO         1| Compile 2 test modules
INFO         1| Run javac with 8 arguments
DEBUG        1| javac --module test.integration,test.programs --module-source-path ./*/test/java --module-path .bach/workspace/modules:.bach/external-modules -d .bach/workspace/classes-test/16
INFO         1| jar(test.integration)
DEBUG        1| jar --create --file .bach/workspace/modules-test/test.integration@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.integration .
INFO         1| jar(test.programs)
DEBUG        1| jar --create --file .bach/workspace/modules-test/test.programs@2.2-ea+ebe4c24+test.jar -C .bach/workspace/classes-test/16/test.programs .
INFO         1| Run junit(test.integration)
DEBUG        1| junit --select-module test.integration --reports-dir .bach/workspace/reports/junit-test/test.integration
INFO         1| Run junit(test.programs)
DEBUG        1| junit --select-module test.programs --reports-dir .bach/workspace/reports/junit-test/test.programs
INFO         1| Build took 6.312s
```

## Thanks for using Bach.java 16-ea+eeddf06

Support its development at <https://github.com/sponsors/sormuras>
