pipeline {
//    agent { docker { image 'mcr.microsoft.com/playwright:v1.43.0-jammy' } }
   stages {
      stage('e2e-tests') {
         steps {
            sh 'npm ci'
            sh 'npx playwright test --list'
            sh 'npx playwright test'
         }
      }
   }
}