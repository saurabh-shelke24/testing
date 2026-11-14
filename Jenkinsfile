pipeline{
agent any{

stages{

  //git connection  
stage(Git connection Test){
    steps{
        Git branch: 'main',
        credentialsID: 'testing-ID',
        url: 'https://github.com/saurabh-shelke24/testing.git'

        echo "Git connection successful"
    }

}

//git all file shows
stage(git show all file){
    steps{
      sh 'ls -la'
      echo "all file shows succesfully"
    }
}


}



}

}