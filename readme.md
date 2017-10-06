## Build Versioning ##

This extension provides a build task to calculate or aquire the build version and to apply the version on several artifacts. Please add this task at the beginning of your build definition.

### Quick steps to get started ###

![](/static/images/Screen1.png)

1. Define the version source and main versioning patterns in the general section.
   - Choose the version source
     - Build Number - Get the version from the current build number (by using macros).
     - Variable - Use a dedicated variable which contains the version information
     - GitVersion - Run (and install) GitVersion and use the calculated version information
     - More to come - Please provide your ideas and requirements at [BuildVersioning Issues](https://github.com/4tecture/BuildVersioning/issues)
  - Define the assembly version pattern and build number format

  ![](/static/images/Screen2.png)
2. Define how to apply the version information to artifacts. Currently supported:
   - .NET Assembly Version
   - Nuspec
   - Npm
   - .NET Core
   - Android (Xamarin)
   - iOS (Xamarin)
   - More to come - Please provide your ideas and requirements at [BuildVersioning Issues](https://github.com/4tecture/BuildVersioning/issues)

  ![](/static/images/Screen3.png)
 
### Known issue(s)
- This extension is currently in preview (beta).
- Installer Url for GitVersion installation does not support redirects (Open Issue at [VSTS Task Tool Lib](https://github.com/Microsoft/vsts-task-tool-lib/)). Please provide a URL without redirection.
- Installer Url has to contain the version information in the ZIP file.

### Learn More

Please visit [Build Versioning](https://github.com/4tecture/BuildVersioning).

### Minimum supported environments ###

- Minimum agent version: 2.123.0


### Feedback ###
- Add a review below.
- Create an issue at [BuildVersioning Issues](https://github.com/4tecture/BuildVersioning/issues)