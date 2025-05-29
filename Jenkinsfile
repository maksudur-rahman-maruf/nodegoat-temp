pipeline {
    agent any
    stages {
        stage("BlackDuckSecruityScan") {
           steps {
               script {
                    security_scan product: "polaris",  
                      polaris_application_name: "maksud-test2", polaris_project_name: "maksud-test2", polaris_test_sast_type: "SAST_FULL",
                      polaris_branch_name: "master", polaris_assessment_types: "SCA,SAST", include_diagnostics: true
                   
               }
           }
       }
    } 
}
