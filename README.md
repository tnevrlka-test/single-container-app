# Simple Container Based App 

## Build containerized app using the App Studio Build Infrastructure 

This repo contains a a simple container based app that can be built on a bootstrapped App Studio build environment.
The application itself can run and shows a simple web page with these same instructions using a simple node.js server to serve up HTML pages. 

Try it out by cloning `https://github.com/redhat-appstudio/infra-deployments.git`  and setting up your cluster to run the build pipeline.
 
| Step    |    |
| ----------- | ----------- |
| 1.  Bootstrap your cluster    |  hack/bootstrap.sh    |
| 2.  Create project for your pipelines execution. This can be run as any non-admin user (or admin)    |  oc new-project demo     |  
| 3.  Run build on this repo.     |  ./components/build/hack/build.sh  https://github.com/jduimovich/single-container-app       |


Login to openshift to view pipelineruns. You may also use the tkn cli to see log `tkn.exe pipelinerun logs`
 


