pipeline {
	agent any
	parameters {
		booleanParam(defaultValue: false, description: "Enable Service..?", name: "myBoolean")
		string(defaultValue: "CRM", description: "application to deploy..?", name: "appName")
		choice(choices: ["TEST", "DEV", "QA", "PRE-PROD", "PROD"], description: "environment to deploy...?", name: "deployEnv")
		choice(choices: ["EU-WEST-2A", "EU-WEST-2B", "EU-WEST-2C"], description: "AZ to deploy...?", name: "azureZone")
	}
	stages {
		stage("stage 1"){
			steps {
				echo "booleanParam is set to: ${params.myBoolean}"
			}
		}
		stage("stage 2"){
			steps {
				echo "application to deploy is: ${params.appName}"
			}
		}
		stage("stage 3"){
			steps {
				echo "environment to deploy is set to: ${params.deployEnv}"
			}
		}
		stage("stage 4"){
			steps {
				echo "AZ to deploy to: ${params.azureZone}"
			}
		}
		stage("stage 5"){
			steps {
				echo "this is task 5"
			}
		}
	}
}
