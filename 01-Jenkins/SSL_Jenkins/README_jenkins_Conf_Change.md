HTTPS_PORT=8443
KEYSTORE="/etc/jenkins/jenkins_keystore.jks"
PASSWORD="redhat@123"


JENKINS_ARGS="--webroot=/var/cache/$NAME/war --httpsPort=$HTTPS_PORT --httpsKeyStore=$KEYSTORE --httpsKeyStorePassword=$PASSWORD --httpPort=-1"
