# spring-gumball ci/cd example

In this lab, I explored how to setup a CI/CD pipeline with github actions, and Google Cloud Platform.

It is especially interesting to see how easily the workflow can not only be managed, but also tested, and deployed with such a pipeline.

The automation tools and the templates provided by github are also quite impressive.

## CI Workflow:

- Set up the CI workflow action to be triggered on push to the main branch.
- It attempts to build the jar file, and on successful completion, it uploads the file.

### Screenshot (CI Workflow)

![ci-workflow](images/CI_Workflow.png)

## CD Workflow

### Screenshots

- GCP Service Accoucnt & JSON Service Account Key

![service-accounts](images/serviceaccount_name.png)

- GitHub Action Secrets

![action-secrets](images/Github_Actions_Secret.png)

- GKE Cluster

![gke-cluster](images/gke_cluster.png)

- V2 Github Release

![v1-release](images/v2.2.png)

- All Github Workflows

![git-workflows](images/all_Actions.png)

# CD Workflow Notes

Unfortunately, I was unable to get the CD workflow to work.

I tried changing a lot of the variables for the authentication section (assuming I got the keys wrong), but it was not working.

Even after trying to get the keys to work, I was unable to get the CD workflow to work.

Hope this could be considered as a GCP account bug.
