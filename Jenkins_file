node{}
stage('SCM Checkout'){
git 'https://github.com/Naveen359-G/Test-file'
}
stage ('Compile-Package'){
// Get maven home path
def mvnHome = tool name: 'maven4', type: 'maven'
sh "${mvnHome}/bin/mvn package"
}
}
