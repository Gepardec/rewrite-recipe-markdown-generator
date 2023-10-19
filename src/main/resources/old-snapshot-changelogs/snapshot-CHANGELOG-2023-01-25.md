## New Recipes
* [org.openrewrite.github.SetupJavaUpgradeJavaVersion](https://docs.openrewrite.org/reference/recipes/github/setupjavaupgradejavaversion): Update the Java version used by `actions/setup-java` if it is below the expected version number. 
* [org.openrewrite.gradle.UpgradeLiteralDependencyVersion](https://docs.openrewrite.org/reference/recipes/gradle/upgradeliteraldependencyversion): A fixed literal version is a version that is not a variable or property or supplied indirectly by platform BOMs or similar means. For example, `com.google.guava:guava:29.0-jre`. 
* [org.openrewrite.gradle.plugins.RemoveBuildPlugin](https://docs.openrewrite.org/reference/recipes/gradle/plugins/removebuildplugin): Remove plugin from `build.gradle(.kts)`. 
* [org.openrewrite.gradle.plugins.RemoveSettingsPlugin](https://docs.openrewrite.org/reference/recipes/gradle/plugins/removesettingsplugin): Remove plugin from `settings.gradle(.kts)`. 
* [org.openrewrite.java.cleanup.ReplaceRedundantFormatWithPrintf](https://docs.openrewrite.org/reference/recipes/java/cleanup/replaceredundantformatwithprintf): Replaces `PrintStream.print(String.format(format, ...args))` with `PrintStream.printf(format, ...args)` (and for `println`, appends a newline to the format string). 
* [org.openrewrite.java.cleanup.SimplifyDurationCreationUnits](https://docs.openrewrite.org/reference/recipes/java/cleanup/simplifydurationcreationunits): Simplifies java.time.Duration units to be more human-readable. 
* [org.openrewrite.java.testing.assertj.UseExplicitSize](https://docs.openrewrite.org/reference/recipes/java/testing/assertj/useexplicitsize): Convert `assertThat(collection.size()).isEqualTo(Y)` with AssertJ's `assertThat(collection).hasSize()`. 

## Changed Recipes
* [org.openrewrite.gradle.search.FindGradleProject](https://docs.openrewrite.org/reference/recipes/gradle/search/findgradleproject) was changed:
  * Old Options:
    * `None`
  * New Options:
    * `searchCriteria: { type: SearchCriteria, required: true }`
* [org.openrewrite.maven.RemoveExclusion](https://docs.openrewrite.org/reference/recipes/maven/removeexclusion) was changed:
  * Old Options:
    * `artifactId: { type: String, required: true }`
    * `exclusionArtifactId: { type: String, required: true }`
    * `exclusionGroupId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
  * New Options:
    * `artifactId: { type: String, required: true }`
    * `exclusionArtifactId: { type: String, required: true }`
    * `exclusionGroupId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
    * `onlyIneffective: { type: Boolean, required: false }`