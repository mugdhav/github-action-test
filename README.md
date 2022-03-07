# Explaining github-action-test contents
This repository contains an example Github Actions workflow, called GitHub Actions Assignment and defined using a .github/workflows/github-actions-demo.yml file.
The workflow contains a single job, called Assignment-GitHub-Actions. This job runs a few steps that print information about:
- The event that triggers this job (push to this repository)
- The operating system this job runs on (ubuntu linux)
- The repository name and branch this job runs on
- And so on

The steps also check out this repository's code to the action runner hosted by GitHub, using the existing ***checkout*** action.
Then the steps also run a few commands that:
- Clone the [example repository](https://github.com/heremaps/maps-api-for-javascript-examples) to this repository.
- Zip all files in the repository into an example_archive file, excluding the workflow and fonts directories. 
- Create a MANIFEST.mf file from the example_archive contents.

The last step prints the final job status.

# Run the workflow and view its result
You can run this workflow and view its result form the Actions tab of this repository. For more details,see [Manually running a workflow](https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow).
