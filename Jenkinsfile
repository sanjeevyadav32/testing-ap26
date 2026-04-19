stage('Detect Changes') {
    steps {
        script {
            def changes = sh(
                script: "git diff --name-only HEAD~1",
                returnStdout: true
            ).trim()

            echo "Changed files: ${changes}"

            if (changes.contains("file1")) {
                echo "Run Job1 logic 🚀"
            }

            if (changes.contains("file2")) {
                echo "Run Job2 logic 🚀"
            }
        }
    }
}
