#!groovy

@Library('share-library') _


def getname = new org.devops.tools()

users = [
			["id": 1, "name": "jenkins1"],
			["id": 2, "name": "jenkins2"],
			["id": 3, "name": "jenkins3"],
		]


pipeline {
    agent any

    stages{
        stage("Test"){
            steps{
                script{
                    
                    name = getname.GetUserNameByID(users,1)
                    print(name)

                  
                    echo "#### vars output demo ####"
                    name = GetUserName(users,2)
                    print(name)


                    //echo "get resources"
                    //data = libraryResource 'config/config.json'
                    //println(data)

                    //data_json = readJSON text: data
                    //println(data_json["id"])
                                   
                }
            }
        }
    }
}
