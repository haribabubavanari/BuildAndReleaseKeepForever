
### Why do we need this plugin?
When a release has successfully deployed to PRODUCTION environment, we wanted to keep that release defintion and all its associated builds forever. This Release task will automate the process.


### Releases
- 1.0.x - Initial release
- 2.0.x - Updated code to work with VSTS also


## Included Tasks
### Build Release Retension Task
This task sets the 'keep forever' retension flag on a Release and its all associated builds. It takes one parameter, the build selection mode, set to either:

* Select only the primary build associated with the release (default)
* All the build artifacts associated with the release
* (Advanced) Use use build agents default credentials as opposed to agent token - usually only every needed for TFS usage 

-- Below is command to create extension 
tfx extension create --manifest-globs vss-extension.json