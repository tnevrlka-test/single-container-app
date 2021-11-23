# Simple Container Based App 

## Build containerized app using the App Studio Build Infrastructure 

This demo shows a simple container based app can easily be bootstrapped onto an openshift cluster.
This application runs a simple node.js server and serves up HTML pages. 

Try it out by cloning `https://github.com/redhat-appstudio/infra-deployments.git`  and setting up your cluster to run the build pipeline.
 
| Step    |    |
| ----------- | ----------- |
| 1.  Bootstrap your cluster    |  hack/bootstrap.sh    |
| 2.  Create project for your pipelines execution    |  oc new-project demo     |
| 3. Install Pipelines       | ./components/build/hack/test-known-build.sh | 
| 4. Test Pipelines     |   ./components/build/hack/test-known-build.sh URL      |
| 5.  Run build on this repo.     |  ./components/build/hack/build.sh  https://github.com/jduimovich/single-container-app       |


Login to openshift to view pipelineruns.
 


