pipeline {
    agent any
    stages {
        stage ('Checking Queen TEST DB Size') {
            steps { 
                echo 'Checking running transactions'
                
            }
        }
        
        stage ( 'Starting Reindexing' ) {

            steps {
        sh script: '/usr/local/bin/psql -d queentestdb -a -f  /reindex_test_db.sql'
                
            }
        }
   
        stage ( 'Reindexing Done On TEST Database' ) {
            steps { 
                echo 'Checks DB Size'
                
            }
        }
    }
}
