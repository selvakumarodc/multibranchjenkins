node('built-in') 
{
    stage('Continuous Download_master') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build in master') 
	{
    sh label: '', script: 'mvn package'
	}
}
