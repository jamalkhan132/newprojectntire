piplene{
    agent any
}
stages{
    stage{
        steps{
            git branch: 'main', url: 'https://github.com/jamalkhan132/springboot-app-main.git'
        }
    }
    post {
		always {
			mail bcc: '', body: "<br>Project: ${env.JOB_NAME} <br>Build Number: ${env.BUILD_NUMBER} <br> URL de build: ${env.BUILD_URL}", cc: '', charset: 'UTF-8', from: '', mimeType: 'text/html', replyTo: '', subject: "${currentBuild.result} CI: Project name -> ${env.JOB_NAME}", to: "jamaldevopsksa@gmail.com";  
		}
	}
}