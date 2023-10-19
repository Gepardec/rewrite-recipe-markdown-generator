## New Recipes
* [org.openrewrite.java.spring.NoRepoAnnotationOnRepoInterface](https://docs.openrewrite.org/reference/recipes/java/spring/norepoannotationonrepointerface): Removes superfluous `@Repository` annotation from Spring Data `Repository` sub-interfaces. 
* [org.openrewrite.java.spring.boot2.MoveAutoConfigurationToImportsFile](https://docs.openrewrite.org/reference/recipes/java/spring/boot2/moveautoconfigurationtoimportsfile): Use `org.springframework.boot.autoconfigure.AutoConfiguration.imports` instead of the deprecated entry `org.springframework.boot.autoconfigure.EnableAutoConfiguration` in `spring.factories` when defining auto-configuration classes. 

## Changed Recipes
* [org.openrewrite.maven.ChangeParentPom](https://docs.openrewrite.org/reference/recipes/maven/changeparentpom) was changed:
  * Old Options:
    * `allowVersionDowngrades: { type: boolean, required: false }`
    * `newArtifactId: { type: String, required: false }`
    * `newGroupId: { type: String, required: false }`
    * `newVersion: { type: String, required: true }`
    * `oldArtifactId: { type: String, required: true }`
    * `oldGroupId: { type: String, required: true }`
    * `versionPattern: { type: String, required: false }`
  * New Options:
    * `allowVersionDowngrades: { type: boolean, required: false }`
    * `newArtifactId: { type: String, required: false }`
    * `newGroupId: { type: String, required: false }`
    * `newVersion: { type: String, required: true }`
    * `oldArtifactId: { type: String, required: true }`
    * `oldGroupId: { type: String, required: true }`
    * `retainVersions: { type: List, required: false }`
    * `versionPattern: { type: String, required: false }`
* [org.openrewrite.maven.UpgradeDependencyVersion](https://docs.openrewrite.org/reference/recipes/maven/upgradedependencyversion) was changed:
  * Old Options:
    * `artifactId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
    * `newVersion: { type: String, required: true }`
    * `overrideManagedVersion: { type: Boolean, required: false }`
    * `versionPattern: { type: String, required: false }`
  * New Options:
    * `artifactId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
    * `newVersion: { type: String, required: true }`
    * `overrideManagedVersion: { type: Boolean, required: false }`
    * `retainVersions: { type: List, required: false }`
    * `versionPattern: { type: String, required: false }`
* [org.openrewrite.maven.UpgradeParentVersion](https://docs.openrewrite.org/reference/recipes/maven/upgradeparentversion) was changed:
  * Old Options:
    * `artifactId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
    * `newVersion: { type: String, required: true }`
    * `versionPattern: { type: String, required: false }`
  * New Options:
    * `artifactId: { type: String, required: true }`
    * `groupId: { type: String, required: true }`
    * `newVersion: { type: String, required: true }`
    * `retainVersions: { type: List, required: false }`
    * `versionPattern: { type: String, required: false }`