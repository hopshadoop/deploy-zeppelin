# Deploy zeppelin

## Deploy zeppelin to sics repository

1.  `cp settings.xml to ~/.m2` 
2.  `git clone git@github.com:apache/zeppelin.git`
3.  Update hadoop and spark versions in deploy.sh if necessary.
4.  `./deploy.sh <path-to-zeppelin> <zeppelin-version> [local|kompics]`

This will build zeppelin and copy the distribution tar to snurran.sics.se. Then add zeppelin-interpreter.jar, zeppelin-zengine.jar, and zeppelin-web.war to 
kompics repository.
