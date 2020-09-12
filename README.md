# README

This is a hello-world example demonstrating how to use github actions in conjunction with the serverless framework
to deploy a lambda function to AWS. 

The github action workflows are defined in `.github/workflows` directory.
The environment variables `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY` and `SERVERLESS_ACCESS_KEY` are all 
added to the repository as secrets through the github UI. I believe there's a way to do this in a nicer way too
but it's not necessary for me at the moment. 

Finally, environment is determined by the branch that is being used. 
The environment variable to use is set by the `::set-env name={env-name}::{env-value}` command.
The documentation for this is here: [Setting an Environment Variable documentation](https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#setting-an-environment-variable)
