node('built-in') 
{
when {
    not {
        expression {
            def causes = currentBuild.getBuildCauses()
            String causesClass = causes._class[0]
            return causesClass.contains('BranchIndexingCause')
        	}
  	  }
	}
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build_loans') 
	{
    sh label: '', script: 'mvn package'
        }	
}
