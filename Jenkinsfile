node {
    stage 'Checkout'
    checkout scm

    stage 'Build'
	def mvnHome = tool 'Maven for DevOps Training'
      	buildStatus= sh returnStatus: true, script:"${mvnHome}/bin/mvn clean package" 
      	echo "Build status : ${buildStatus}"

   
} 
