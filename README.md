### Spotter upgrade scenario with CI pipeline
This is an upgrade case demo for steampunk spotter. 
It is meant to show how we can upgrade the playbooks from an older ansible version to a newer one. 
This also includes the CI pipeline and demonstrates how developers can include scanning into their pipelines and help with pull requests. 

If you want to use this repository it is best to fork this. 
# Steps: 
- Create a new project in Spotter web interface with this Git repo
- Inspect the first scan
- Open the cloned project in prefered editor
- run `spotter scan . --ansible-version 2.16`
- show how the output is the same as in the web version
- run `spotter scan . --ansible-version 2.16 --rewrite` to show the rewrite capability of spotter
- commit and push the changes
- rerun the scan from the web interface
- show how many errors can be fixed when migrating to a newer version
- show how the errors can be fixed with the help of spotter
- example: `Value of provider in module openssl_certificate is set to assertonly which does not match any of the possible choices listed in [acme, entrust, ownca, selfsigned] `
- go back to the git repository and create a PR
- show the output of the pipeline
# Example of the pipeline output
![image](https://github.com/user-attachments/assets/2dff4e20-b785-48fc-ac25-7516f1ce73c6)








