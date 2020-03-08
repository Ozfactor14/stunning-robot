pipeline {
  agent none
  stages {
    stage('Scan for O.S') {
      parallel {
        stage('Windows') {
          steps {
            echo 'Check Windows'
          }
        }

        stage('Linux') {
          steps {
            echo 'Check Linux'
          }
        }

        stage('Mac') {
          steps {
            echo 'Check Mac'
          }
        }

        stage('VM 1') {
          steps {
            echo 'VM1'
          }
        }

        stage('VM 2') {
          steps {
            echo 'VM2'
          }
        }

      }
    }

    stage('Prep') {
      parallel {
        stage('WIndows') {
          steps {
            echo 'Prep WIndows'
          }
        }

        stage('Linux') {
          steps {
            echo 'Build '
          }
        }

        stage('Mac') {
          steps {
            echo 'Build Mac'
          }
        }

        stage('Vm 1') {
          steps {
            echo 'Prep Vm1'
          }
        }

        stage('Vm2') {
          steps {
            echo 'VM 2'
          }
        }

      }
    }

    stage('Build') {
      parallel {
        stage('Windows') {
          steps {
            echo 'Build'
          }
        }

        stage('Linux') {
          steps {
            echo 'j'
          }
        }

      }
    }

    stage('Test') {
      parallel {
        stage('Windows') {
          steps {
            echo 's'
          }
        }

        stage('Linux') {
          steps {
            echo 'w'
          }
        }

      }
    }

    stage('Scan') {
      parallel {
        stage('Windows') {
          steps {
            echo '1'
            echo '"oss"'
          }
        }

        stage('Linux') {
          steps {
            echo '2'
          }
        }

      }
    }

    stage('Post') {
      parallel {
        stage('Windows') {
          steps {
            echo '1'
          }
        }

        stage('Linux') {
          steps {
            echo '2'
          }
        }

      }
    }

  }
}