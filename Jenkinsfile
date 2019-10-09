node {
  try {
    stage('checkout') {
      checkout scm
    }
    stage('prepare') {
      bat "git clean -fdx"
    }
    stage('compile') {
      echo "nothing to compile for hello.sh..."
    }
    stage('test') {
      bat "./test_hello.sh"
    }
    stage('package') {
      bat "tar -cvzf hello.tar.gz hello.sh"
    }
    stage('publish') {
      echo "uploading package..."
    }
  } finally {
    stage('cleanup') {
      echo "doing some cleanup..."
    }
  }
