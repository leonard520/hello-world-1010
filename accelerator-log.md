# Accelerator Log

## Options
```json
{
  "projectName" : "hello-world-1010",
  "projectType" : "maven"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Include, Exclude, Chain(Merge(merge), UniquePath(UseLast)))
┃ ┃ engine.transformations[0].<combo> (Chain)
┃ ┃  Info Running Chain(Include, Exclude, Chain)
┃ ┃ ┏ engine.transformations[0].<combo>.transformations[0] (Include)
┃ ┃ ┃  Info Will include [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties]
┃ ┃ ┃ Debug .gitignore didn't match [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> excluded
┃ ┃ ┃ Debug README.md matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug asc.png didn't match [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> excluded
┃ ┃ ┃ Debug build.gradle matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug checkstyle/checkstyle.xml matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug checkstyle/format.xml matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug pom.xml matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug settings.gradle matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┃ Debug src/main/java/io/cloudevents/examples/springboot/Application.java matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┗ Debug src/main/resources/application.properties matched [**/*.md, **/*.xml, **/*.gradle, **/*.java, **/*.properties] -> included
┃ ┃ ┏ engine.transformations[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃  Info Will exclude [*.png]
┃ ┃ ┃ Debug README.md didn't match [*.png] -> included
┃ ┃ ┃ Debug build.gradle didn't match [*.png] -> included
┃ ┃ ┃ Debug checkstyle/checkstyle.xml didn't match [*.png] -> included
┃ ┃ ┃ Debug checkstyle/format.xml didn't match [*.png] -> included
┃ ┃ ┃ Debug pom.xml didn't match [*.png] -> included
┃ ┃ ┃ Debug settings.gradle didn't match [*.png] -> included
┃ ┃ ┃ Debug src/main/java/io/cloudevents/examples/springboot/Application.java didn't match [*.png] -> included
┃ ┃ ┗ Debug src/main/resources/application.properties didn't match [*.png] -> included
┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2] (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#projectType == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#projectType == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.xml]
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/*.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug checkstyle/checkstyle.xml matched [**/*.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug checkstyle/format.xml matched [**/*.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**/*.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/*.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/io/cloudevents/examples/springboot/Application.java didn't match [**/*.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/main/resources/application.properties didn't match [**/*.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [artifactIdName->hello-world-1010]
┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#projectType == 'gradle') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ engine.transformations[0].<combo>.transformations[2].transformations[0].sources[2].include (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**/*.java, README.md, **/*.properties]
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**/*.java, README.md, **/*.properties] -> included
┃ ┃ ┃ ┃ ┃ Debug build.gradle didn't match [**/*.java, README.md, **/*.properties] -> excluded
┃ ┃ ┃ ┃ ┃ Debug checkstyle/checkstyle.xml didn't match [**/*.java, README.md, **/*.properties] -> excluded
┃ ┃ ┃ ┃ ┃ Debug checkstyle/format.xml didn't match [**/*.java, README.md, **/*.properties] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java, README.md, **/*.properties] -> excluded
┃ ┃ ┃ ┃ ┃ Debug settings.gradle didn't match [**/*.java, README.md, **/*.properties] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/io/cloudevents/examples/springboot/Application.java matched [**/*.java, README.md, **/*.properties] -> included
┃ ┃ ┃ ┗ ┗ Debug src/main/resources/application.properties matched [**/*.java, README.md, **/*.properties] -> included
┃ ┗ ┗ ╺ engine.transformations[0].<combo>.transformations[2].transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
