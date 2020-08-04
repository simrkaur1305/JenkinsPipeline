pipeline {
  agent { label 'master' }
  stages {
    stage('Restricted Correction Policy') {
      steps {
          sh '''#!/bin/bash
                export LD_LIBRARY_PATH=/build/trssdkroot/automation_scripts/python/ssl/lib/:$LD_LIBRARY_PATH
                export LD_LIBRARY_PATH=/build/trssdkroot/automation_scripts/python/libfii/lib64/:$LD_LIBRARY_PATH
                export PATH=/build/trssdkroot/automation_scripts/python/python3/bin:$PATH
                export PYTHONPATH=/build/trssdkroot/automation_scripts/python/python3
                $PYTHONPATH/bin/python3.8 /home/simrkaur/scripts/restricted_correction_policy/main.py
                '''
      }
    }
}
}

