#### jenkins-shared-library

### sample jenkins shared library to automate jobs in pipeline

## (3) Creating shared library

Added empty git repo: https://github.com/njain50/jenkins-shared-library

This is how our shared library dir structure looks like: 
├── jenkins-shared-library
│   ├── src
│   │   ├── org
│   │   │   ├── example
│   ├── vars

git clone and open in IntelliJ. 
Create dir structure same as above. 

(4) In Jenkins, go to Manage Jenkins &rarr; Configure System. Under _Global Pipeline Libraries_, add a library with the following settings:
    
        - Name: `pipeline-library-demo`
        - Default version: Specify a Git reference (branch or commit SHA), e.g. `master`
        - Retrieval method: _Modern SCM_
        - Select the _Git_ type
        - Project repository: `https://github.com/monodot/pipeline-library-demo.git`
        - Credentials: (leave blank)
 


