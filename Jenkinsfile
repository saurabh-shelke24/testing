pipeline{
agent any

stages{

  //git connection  
stage('Git connection Test'){
    steps{
        git branch: 'main',
        credentialsId: 'testing-ID',
        url: 'https://github.com/saurabh-shelke24/testing.git'

        echo "Git connection successful"
    }

}

//git all file shows
stage('git show all file'){
    steps{
      sh 'ls -la'
      echo "all file are showened succefully"
    }
}

stage('latest commit'){
    steps{
        checkout scm
        echo "checkout file successful"
    }
}

stage('git check required file'){
    steps{
        sh 'ls -la'
        sh 'test -f index.html'
        sh 'test -f Dockerfile'
        echo "Git check file successful"
    }
}

//Docker image creation
stage('Docker image creation'){
    steps{
        sh 'docker build -t testing:latest .'
        echo "Docker image creation successful"
    }
}

//docker container creation
stage('docker container creation'){
    steps{
        sh 'docker rm -f testing || true'
        sh 'docker run -d --name testing --restart  unless-stopped -p 80:80 testing:latest'
        echo "container deployment successful"
    }
}
}

}