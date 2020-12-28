pipeline {
    agent any
    stages {
        stage ('Checking BuyQ TEST DB Size') {
            steps { 
                echo 'Checking running transactions'
                
            }
        }
        
        
        stage ( 'Starting Reindexing' ) {
            steps {
        sh script:'/usr/local/bin/psql -d buyqtestdb -a -f  /Users/raheman/MSMr/BUYQ_Project/reindex_test_db.sql'
                
            }
        }
   
        stage ( 'Reindexing Done On Database' ) {
            steps { 
                echo 'Checks DB Size'
                
            }
        }
    }
}
