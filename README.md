# CumulusCI GitHub Action
- CumulusCI GitHub Action to be used for on Platform Salesforce projects that have already set up CumulusCI.

# Setup
- First setup CumulusCI for your repo: https://cumulusci.readthedocs.io/en/latest/tutorial.html
- Create a new file in `.github/workflows/` called "feature_tests.yml"
- Copy action into file.
- Replace `<replacewithprojectname>` with CumulusCI Project Name (note: refer to `robot` folder in project for name)
- Create a GitHub Personal Access Token: https://github.com/settings/tokens/new
- Add the token to GitHub repo secrets and name it `CUMULUSCI_SERVICE_github`
- Run `sfdx force:org:display --verbose -u <devhubusername>` for your devhub
- Add `Sfdx Auth Url` to GitHub repo secrets and name it `SFDX_AUTH_URL` 

# Need Help?
- Refer to https://cumulusci.readthedocs.io/en/latest/cookbook.html#continuous-integration-with-cumulusci-and-github-actions

# Credits
- Action is based on work by @davisagli and the Salesforce.org Release Engineering Team
