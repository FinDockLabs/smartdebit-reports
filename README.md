<a href="https://githubsfdeploy.herokuapp.com">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

# SmartDebit report duplicates

Created by: [Chris Boxall (FinDock)](https://www.linkedin.com/in/chris-boxall-4144b5a5/)
Contact: `chris@findock.com`

With Smart Debit automated reports we poll for BACS reports daily, these reports will duplicate for a few days while they are still available within the poll request. We already ensure that no action is taken on duplicates but this flow is designed to run daily and change the status of any duplicates so you can recognise them and respond. You can choose to delete duplicates and ensure any other scheduled flows that could be triggered off the back of inbound reports don’t run.

Repository contains
- One scheduled Flow to loop through and flag duplicate BACS reports

Requirements
- BACS for FinDock package installed

## Installation / Deployment

Simply install and activate the flow.
To deploy the flow to your Salesforce environment, you can:
- use `sf` cli.
- press the "Deploy to Salesforce" button at the top of this README and then press "Login to Salesforce" in the top right of your screen.
- any other deployment method you prefer.

## Contributing

When contributing to this repository, please first discuss the change you wish to make via an issue or any other method with FinDock before making a change.

## Support

FinDock Labs is a non-supported group in FinDock that releases applications. Despite the name, assistance for any of these applications is not provided by FinDock Support because they are not officially supported features. For a list of these apps, visit the FinDock Labs account on Github. 

## License

This project is licensed under the MIT License - see the [LICENSE](/LICENSE) file for details