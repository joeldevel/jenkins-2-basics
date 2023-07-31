# jenkins-2-basics
Learning Jenkins2, groovy, etc.

## Pipeline syntax (script) example

```groovy
node () {
  stage('Source') {
    git branch: 'main', url: 'https://github.com/joeldevel/jenkins-2-basics.git'
  }
  stage('Greetings') {
    sh 'echo "Bonjour cornutti!"'
  }
}

```
