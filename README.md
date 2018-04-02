# USAGE

## Build and deploy archetype to artefactory

- mvn archetype:create-from-project
- cd target/generated-sources/archetype
- mvn versions:set -DnewVersion=20180310
- mvn deploy

## Intellij setup

- Add to archetype file manually. E.g. on a mac
- vi /Users/stittp/Library/Caches/IntelliJIdea2017.3/Maven/Indices/UserArchetypes.xml
Add/Edit to get something like:
```xml
    <archetypes>
         <archetype groupId="com.rentalcars.stittp" artifactId="java8tddArchetype-archetype" version="20170310" />
    </archetypes>
```
- Create a new project, tick from archetype, then choose archetype
