# es7-ivy-repo

Testing a project with offline IVY repository using gradle plugin `org.ysb33r.ivypot`


## See dependencies of module `app`

```
./gradlew app::dependencies --configuration runtimeClasspath
```

There we can see for example:
```
com.carrotsearch:hppc:0.8.1
org.apache.lucene:lucene-core:8.7.0
```


## Sync remote repositories using the `org.ysb33r.ivypot` plugin

```
./gradlew sync:syncRemoteRepositories
```

Observe the JARs that were synchronized to `sync/build/ivyrepo`:

There are no JARs in e.g.:
- `com.carrotsearch/hppc/0.8.1`
- `org.apache.lucene/lucene-core/8.7.0`
