// Powered by Infostretch 

timestamps {

node () {

	stage ('README_UPDATER_FREESTYLE - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '7f0e8a8a-5a23-4df7-8db8-cecc3e50a5f4', url: 'https://github.com/Omkar76/BTITA78_onkar']]]) 
	}
	stage ('README_UPDATER_FREESTYLE - Build') {
 	
// Unable to convert a build step referring to "org.jenkinsci.plugins.credentialsbinding.impl.SecretBuildWrapper". Please verify and convert manually if required.		// Shell build step
sh """ 
echo "This file is periodically updated by jenkins. Last updated $(date)" > README.md
git add README.md
git commit -m "Updated from jenkins" 
 """ 
	}
}
}