# SevenSins plugin build

This project targets Java 21 and Paper API 1.21.11.

## Build on GitHub Actions

1. Upload the contents of this ZIP to the root of your GitHub repository, preserving the `.github` and `SevenSins` folders.
2. If your repository already has `.github/workflows/build.yml`, replace it with the included workflow.
3. Commit the changes and open the repository's **Actions** tab.
4. Open the latest **Build SevenSins Plugin** run. After a successful green check, download `SevenSins-jar` under **Artifacts**.
5. Extract the downloaded ZIP. The plugin file is `SevenSins-1.0.0.jar`.

## Build locally

Install Java 21 and Maven. In a terminal, enter the `SevenSins` folder and run:

```sh
mvn clean package
```

The generated JAR will be at `SevenSins/target/SevenSins-1.0.0.jar` relative to the repository root.

## Important

This ZIP contains the Java plugin source and configuration files. It does not contain a separate custom resource pack or texture files. The build is configured for Paper 1.21.11; use a compatible Paper server version.
