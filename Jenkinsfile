#!/usr/bin/env groovy
/** This is a test pipeline

*/
import hudson.model.*
import hudson.EnvVars
import groovy.json.JsonSlurperClassic
import groovy.json.JsonBuilder
import groovy.json.JsonOutput
import java.net.URL

try {

node {

	stage '\u2776 Scm Checkout'
	def GitHome = tool name: 'git', type: 'git'
	def GitCmd = "${GitHome}/bin/git"
	${GitCmd} (credentialsId: 'git-credentials-id', url: 'https://github.com/jibinjose087/encryption_code.git', branch: 'stage')
	echo ${GitCmd}
	which git
}

}

catch (exec) {


}

finally {

}
