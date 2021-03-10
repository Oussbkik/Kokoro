# Kokoro
ty-4bcd4.appspot.com
﻿Warning: Permanently added 'localhost' (ECDSA) to the list of known hosts.
Warning: Permanently added 'localhost' (ECDSA) to the list of known hosts.
Warning: Permanently added 'localhost' (ECDSA) to the list of known hosts.
[02:31:30] Transferring environment variable script to build VM
[02:31:31] Transferring kokoro_log_reader.py to build VM
[02:31:32] Transferring source code to build VM
[02:31:37] Executing build script on build VM



[ID: 7364974] Executing command via SSH:
export KOKORO_BUILD_NUMBER="358"
export KOKORO_JOB_NAME="cloud-devrel/client-libraries/java/java-video-intelligence/nightly/java7"
source /tmpfs/kokoro-env_vars.sh; cd /tmpfs/src/ ;  chmod 755 github/java-video-intelligence/.kokoro/trampoline.sh ;  nohup bash -c "( rm -f /tmpfs/kokoro_build_exit_code ; github/java-video-intelligence/.kokoro/trampoline.sh   ; echo \${PIPESTATUS[0]} > /tmpfs/kokoro_build_exit_code ) > /tmpfs/kokoro_build.log 2>&1" > /dev/null 2>&1 & echo $! > /tmpfs/kokoro_build.pid ; python /tmpfs/kokoro_log_reader.py /tmpfs/kokoro_build.log /tmpfs/kokoro_build_exit_code /tmpfs/kokoro_build.pid /tmpfs/kokoro_log_reader.pid --start_byte 0

2021-02-19 02:31:37 Creating folder on disk for secrets: /tmpfs/src/gfile/secret_manager
Activated service account credentials for: [kokoro-trampoline@cloud-devrel-kokoro-resources.iam.gserviceaccount.com]
WARNING: Your config file at [/home/kbuilder/.docker/config.json] contains these credential helper entries:

{
  "credHelpers": {
    "gcr.io": "gcr", 
    "us.gcr.io": "gcr", 
    "asia.gcr.io": "gcr", 
    "staging-k8s.gcr.io": "gcr", 
    "eu.gcr.io": "gcr"
  }
}
These will be overwritten.
Docker configuration file updated.
Using default tag: latest
latest: Pulling from cloud-devrel-kokoro-resources/java7
f2b6b4884fc8: Pulling fs layer
4fb899b4df21: Pulling fs layer
74eaa8be7221: Pulling fs layer
e7be20ca4c60: Pulling fs layer
6a8a0c25768c: Pulling fs layer
b8449367f126: Pulling fs layer
7c7f86153417: Pulling fs layer
61b90d887704: Pulling fs layer
291c69af0b71: Pulling fs layer
d2e5e3ca94ce: Pulling fs layer
db6dc44cf96a: Pulling fs layer
036f3d99bef8: Pulling fs layer
f60ed14351ef: Pulling fs layer
61fbc01edf8c: Pulling fs layer
72727bb52dd3: Pulling fs layer
01e2fbe70096: Pulling fs layer
e032ded037b7: Pulling fs layer
c44b7cdea0a3: Pulling fs layer
84389f7d0c49: Pulling fs layer
3ba1def1143e: Pulling fs layer
6a8a0c25768c: Waiting
b8449367f126: Waiting
7c7f86153417: Waiting
61b90d887704: Waiting
291c69af0b71: Waiting
e7be20ca4c60: Waiting
d2e5e3ca94ce: Waiting
db6dc44cf96a: Waiting
036f3d99bef8: Waiting
f60ed14351ef: Waiting
61fbc01edf8c: Waiting
72727bb52dd3: Waiting
01e2fbe70096: Waiting
e032ded037b7: Waiting
c44b7cdea0a3: Waiting
84389f7d0c49: Waiting
3ba1def1143e: Waiting
4fb899b4df21: Verifying Checksum
4fb899b4df21: Download complete
e7be20ca4c60: Verifying Checksum
e7be20ca4c60: Download complete
6a8a0c25768c: Verifying Checksum
6a8a0c25768c: Download complete
f2b6b4884fc8: Verifying Checksum
f2b6b4884fc8: Download complete
b8449367f126: Verifying Checksum
b8449367f126: Download complete
74eaa8be7221: Verifying Checksum
74eaa8be7221: Download complete
61b90d887704: Verifying Checksum
61b90d887704: Download complete
d2e5e3ca94ce: Verifying Checksum
d2e5e3ca94ce: Download complete
291c69af0b71: Verifying Checksum
291c69af0b71: Download complete
7c7f86153417: Verifying Checksum
7c7f86153417: Download complete
db6dc44cf96a: Verifying Checksum
db6dc44cf96a: Download complete
f60ed14351ef: Verifying Checksum
f60ed14351ef: Download complete
61fbc01edf8c: Verifying Checksum
61fbc01edf8c: Download complete
01e2fbe70096: Verifying Checksum
01e2fbe70096: Download complete
e032ded037b7: Verifying Checksum
e032ded037b7: Download complete
036f3d99bef8: Verifying Checksum
036f3d99bef8: Download complete
f2b6b4884fc8: Pull complete
72727bb52dd3: Verifying Checksum
72727bb52dd3: Download complete
3ba1def1143e: Verifying Checksum
3ba1def1143e: Download complete
4fb899b4df21: Pull complete
c44b7cdea0a3: Download complete
84389f7d0c49: Verifying Checksum
84389f7d0c49: Download complete
74eaa8be7221: Pull complete
e7be20ca4c60: Pull complete
6a8a0c25768c: Pull complete
b8449367f126: Pull complete
7c7f86153417: Pull complete
61b90d887704: Pull complete
291c69af0b71: Pull complete
d2e5e3ca94ce: Pull complete
db6dc44cf96a: Pull complete
036f3d99bef8: Pull complete
f60ed14351ef: Pull complete
61fbc01edf8c: Pull complete
72727bb52dd3: Pull complete
01e2fbe70096: Pull complete
e032ded037b7: Pull complete
c44b7cdea0a3: Pull complete
84389f7d0c49: Pull complete
3ba1def1143e: Pull complete
Digest: sha256:b4e8e23dbd101ccfd88c6b9315b04f806375775cb360a9ecd374a225d8299559
Status: Downloaded newer image for gcr.io/cloud-devrel-kokoro-resources/java7:latest
Executing: docker run --rm --interactive --network=host --privileged --volume=/var/run/docker.sock:/var/run/docker.sock --workdir=/tmpfs/src --entrypoint=github/java-video-intelligence/.kokoro/build.sh --env-file=/tmpfs/tmp/tmp4e6edr77/envfile --volume=/tmpfs:/tmpfs gcr.io/cloud-devrel-kokoro-resources/java7
java version "1.7.0_151"
OpenJDK Runtime Environment (IcedTea 2.6.11) (7u151-2.6.11-2~deb8u1)
OpenJDK 64-Bit Server VM (build 24.151-b01, mixed mode)
test
Apache Maven 3.6.3 (cecedd343002696d0abb50b32b541b8a6ba2883f)
Maven home: /usr/local/lib/maven
Java version: 1.7.0_151, vendor: Oracle Corporation, runtime: /usr/lib/jvm/java-7-openjdk-amd64/jre
Default locale: en, platform encoding: UTF-8
OS name: "linux", version: "4.15.16-041516-generic", arch: "amd64", family: "unix"
[INFO] Scanning for projects...
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-config/0.10.0/google-cloud-shared-config-0.10.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-config/0.10.0/google-cloud-shared-config-0.10.0.pom (32 kB at 86 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plugins/nexus-staging-maven-plugin/1.6.8/nexus-staging-maven-plugin-1.6.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plugins/nexus-staging-maven-plugin/1.6.8/nexus-staging-maven-plugin-1.6.8.pom (12 kB at 442 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-staging/1.6.8/nexus-staging-1.6.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-staging/1.6.8/nexus-staging-1.6.8.pom (2.8 kB at 110 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-maven-plugins/1.6.8/nexus-maven-plugins-1.6.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-maven-plugins/1.6.8/nexus-maven-plugins-1.6.8.pom (18 kB at 627 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/6/public-parent-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/6/public-parent-6.pom (760 B at 36 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/6/buildsupport-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/6/buildsupport-6.pom (23 kB at 884 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-common/1.6.8/nexus-common-1.6.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-common/1.6.8/nexus-common-1.6.8.pom (2.2 kB at 93 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.4/plexus-sec-dispatcher-1.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.4/plexus-sec-dispatcher-1.4.pom (3.0 kB at 135 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/12/spice-parent-12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/12/spice-parent-12.pom (6.8 kB at 324 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/4/forge-parent-4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/4/forge-parent-4.pom (8.4 kB at 365 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.7/plexus-cipher-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.7/plexus-cipher-1.7.pom (4.2 kB at 199 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/15/spice-parent-15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/15/spice-parent-15.pom (8.4 kB at 363 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/14.0.1/guava-14.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/14.0.1/guava-14.0.1.pom (5.4 kB at 244 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/14.0.1/guava-parent-14.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/14.0.1/guava-parent-14.0.1.pom (2.6 kB at 116 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/oss/oss-parent/7/oss-parent-7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/oss/oss-parent/7/oss-parent-7.pom (4.8 kB at 230 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-client-core/2.14.3-02/nexus-client-core-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-client-core/2.14.3-02/nexus-client-core-2.14.3-02.pom (4.9 kB at 205 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-components/2.14.3-02/nexus-components-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-components/2.14.3-02/nexus-components-2.14.3-02.pom (2.6 kB at 118 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-parent/2.14.3-02/nexus-parent-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-parent/2.14.3-02/nexus-parent-2.14.3-02.pom (38 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/9/public-parent-9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/9/public-parent-9.pom (760 B at 33 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/9/buildsupport-9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/9/buildsupport-9.pom (24 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/buildsupport/nexus-buildsupport-all/2.14.3-02/nexus-buildsupport-all-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/buildsupport/nexus-buildsupport-all/2.14.3-02/nexus-buildsupport-all-2.14.3-02.pom (6.5 kB at 308 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/buildsupport/nexus-buildsupport/2.14.3-02/nexus-buildsupport-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/buildsupport/nexus-buildsupport/2.14.3-02/nexus-buildsupport-2.14.3-02.pom (2.2 kB at 103 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-commons/2.14.3-02/nexus-buildsupport-commons-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-commons/2.14.3-02/nexus-buildsupport-commons-2.14.3-02.pom (3.1 kB at 7.3 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-db/2.14.3-02/nexus-buildsupport-db-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-db/2.14.3-02/nexus-buildsupport-db-2.14.3-02.pom (3.2 kB at 23 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-gwt/2.14.3-02/nexus-buildsupport-gwt-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-gwt/2.14.3-02/nexus-buildsupport-gwt-2.14.3-02.pom (2.2 kB at 15 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-httpclient/2.14.3-02/nexus-buildsupport-httpclient-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-httpclient/2.14.3-02/nexus-buildsupport-httpclient-2.14.3-02.pom (2.1 kB at 15 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-insight/2.14.3-02/nexus-buildsupport-insight-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-insight/2.14.3-02/nexus-buildsupport-insight-2.14.3-02.pom (4.4 kB at 31 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-maven/2.14.3-02/nexus-buildsupport-maven-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-maven/2.14.3-02/nexus-buildsupport-maven-2.14.3-02.pom (7.1 kB at 49 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-messaging/2.14.3-02/nexus-buildsupport-messaging-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-messaging/2.14.3-02/nexus-buildsupport-messaging-2.14.3-02.pom (5.0 kB at 33 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-shiro/2.14.3-02/nexus-buildsupport-shiro-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-shiro/2.14.3-02/nexus-buildsupport-shiro-2.14.3-02.pom (3.4 kB at 24 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-bouncycastle/2.14.3-02/nexus-buildsupport-bouncycastle-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-bouncycastle/2.14.3-02/nexus-buildsupport-bouncycastle-2.14.3-02.pom (2.1 kB at 15 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-jetty/2.14.3-02/nexus-buildsupport-jetty-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-jetty/2.14.3-02/nexus-buildsupport-jetty-2.14.3-02.pom (4.5 kB at 31 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-goodies/2.14.3-02/nexus-buildsupport-goodies-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-goodies/2.14.3-02/nexus-buildsupport-goodies-2.14.3-02.pom (3.6 kB at 25 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-groovy/2.14.3-02/nexus-buildsupport-groovy-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-groovy/2.14.3-02/nexus-buildsupport-groovy-2.14.3-02.pom (3.1 kB at 22 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-guice/2.14.3-02/nexus-buildsupport-guice-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-guice/2.14.3-02/nexus-buildsupport-guice-2.14.3-02.pom (3.7 kB at 26 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-logging/2.14.3-02/nexus-buildsupport-logging-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-logging/2.14.3-02/nexus-buildsupport-logging-2.14.3-02.pom (3.3 kB at 24 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-osgi/2.14.3-02/nexus-buildsupport-osgi-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-osgi/2.14.3-02/nexus-buildsupport-osgi-2.14.3-02.pom (2.0 kB at 15 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-other/2.14.3-02/nexus-buildsupport-other-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-other/2.14.3-02/nexus-buildsupport-other-2.14.3-02.pom (7.0 kB at 50 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-plexus/2.14.3-02/nexus-buildsupport-plexus-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-plexus/2.14.3-02/nexus-buildsupport-plexus-2.14.3-02.pom (4.5 kB at 32 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-rest/2.14.3-02/nexus-buildsupport-rest-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-rest/2.14.3-02/nexus-buildsupport-rest-2.14.3-02.pom (5.1 kB at 36 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-testing/2.14.3-02/nexus-buildsupport-testing-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-testing/2.14.3-02/nexus-buildsupport-testing-2.14.3-02.pom (5.0 kB at 36 kB/s)
[INFO] Downloading from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-metrics/2.14.3-02/nexus-buildsupport-metrics-2.14.3-02.pom
[INFO] Downloaded from rso-public-grid: https://repository.sonatype.org/content/groups/sonatype-public-grid/org/sonatype/nexus/buildsupport/nexus-buildsupport-metrics/2.14.3-02/nexus-buildsupport-metrics-2.14.3-02.pom (3.0 kB at 22 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-restlet1x-model/2.14.3-02/nexus-restlet1x-model-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-restlet1x-model/2.14.3-02/nexus-restlet1x-model-2.14.3-02.pom (3.5 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-plugins-restlet1x/2.14.3-02/nexus-plugins-restlet1x-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-plugins-restlet1x/2.14.3-02/nexus-plugins-restlet1x-2.14.3-02.pom (6.0 kB at 300 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-plugins/2.14.3-02/nexus-plugins-2.14.3-02.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-plugins/2.14.3-02/nexus-plugins-2.14.3-02.pom (32 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.4/maven-model-3.0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.4/maven-model-3.0.4.pom (3.8 kB at 200 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0.4/maven-3.0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0.4/maven-3.0.4.pom (22 kB at 840 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.7/slf4j-api-1.7.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.7/slf4j-api-1.7.7.pom (2.7 kB at 134 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.7.7/slf4j-parent-1.7.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.7.7/slf4j-parent-1.7.7.pom (12 kB at 595 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/2.0.1/jsr305-2.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/2.0.1/jsr305-2.0.1.pom (965 B at 51 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/intellij/annotations/9.0.4/annotations-9.0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/intellij/annotations/9.0.4/annotations-9.0.4.pom (1.2 kB at 66 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.pom (10 kB at 535 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/25/commons-parent-25.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/25/commons-parent-25.pom (48 kB at 1.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/9/apache-9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/9/apache-9.pom (15 kB at 722 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream/1.4.7/xstream-1.4.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream/1.4.7/xstream-1.4.7.pom (11 kB at 535 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream-parent/1.4.7/xstream-parent-1.4.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream-parent/1.4.7/xstream-parent-1.4.7.pom (26 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/codehaus-parent/3/codehaus-parent-3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/codehaus-parent/3/codehaus-parent-3.pom (4.1 kB at 196 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xmlpull/xmlpull/1.1.3.1/xmlpull-1.1.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xmlpull/xmlpull/1.1.3.1/xmlpull-1.1.3.1.pom (386 B at 18 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xpp3/xpp3_min/1.1.4c/xpp3_min-1.1.4c.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xpp3/xpp3_min/1.1.4c/xpp3_min-1.1.4c.pom (1.6 kB at 80 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/joda-time/joda-time/2.2/joda-time-2.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/joda-time/joda-time/2.2/joda-time-2.2.pom (16 kB at 735 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-beanutils/commons-beanutils-core/1.8.3/commons-beanutils-core-1.8.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-beanutils/commons-beanutils-core/1.8.3/commons-beanutils-core-1.8.3.pom (1.6 kB at 86 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-client/1.7/siesta-client-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-client/1.7/siesta-client-1.7.pom (1.8 kB at 101 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta/1.7/siesta-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta/1.7/siesta-1.7.pom (12 kB at 575 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/5/public-parent-5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/public-parent/5/public-parent-5.pom (760 B at 40 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/5/buildsupport-5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/buildsupport/buildsupport/5/buildsupport-5.pom (22 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-common/1.7/siesta-common-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-common/1.7/siesta-common-1.7.pom (2.1 kB at 107 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/ws/rs/jsr311-api/1.1.1/jsr311-api-1.1.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/ws/rs/jsr311-api/1.1.1/jsr311-api-1.1.1.pom (5.5 kB at 288 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-core/1.17.1/jersey-core-1.17.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-core/1.17.1/jersey-core-1.17.1.pom (10 kB at 520 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-project/1.17.1/jersey-project-1.17.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-project/1.17.1/jersey-project-1.17.1.pom (21 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/net/java/jvnet-parent/1/jvnet-parent-1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/net/java/jvnet-parent/1/jvnet-parent-1.pom (4.7 kB at 248 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.pom (7.9 kB at 271 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-client/1.17.1/jersey-client-1.17.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-client/1.17.1/jersey-client-1.17.1.pom (6.7 kB at 279 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-apache-client4/1.17.1/jersey-apache-client4-1.17.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-apache-client4/1.17.1/jersey-apache-client4-1.17.1.pom (6.2 kB at 296 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-contribs/1.17.1/jersey-contribs-1.17.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-contribs/1.17.1/jersey-contribs-1.17.1.pom (3.6 kB at 137 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.3.5/httpclient-4.3.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.3.5/httpclient-4.3.5.pom (5.2 kB at 237 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-client/4.3.5/httpcomponents-client-4.3.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-client/4.3.5/httpcomponents-client-4.3.5.pom (15 kB at 223 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/project/7/project-7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/project/7/project-7.pom (27 kB at 973 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.3.2/httpcore-4.3.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.3.2/httpcore-4.3.2.pom (4.6 kB at 118 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-core/4.3.2/httpcomponents-core-4.3.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-core/4.3.2/httpcomponents-core-4.3.2.pom (12 kB at 169 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.6/commons-codec-1.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.6/commons-codec-1.6.pom (11 kB at 507 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/22/commons-parent-22.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/22/commons-parent-22.pom (42 kB at 1.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.7.7/jcl-over-slf4j-1.7.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.7.7/jcl-over-slf4j-1.7.7.pom (1.9 kB at 93 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-jackson/1.7/siesta-jackson-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-jackson/1.7/siesta-jackson-1.7.pom (2.6 kB at 142 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.1/jackson-annotations-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.1/jackson-annotations-2.3.1.pom (1.7 kB at 95 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/11/oss-parent-11.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/11/oss-parent-11.pom (23 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.3.1/jackson-core-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.3.1/jackson-core-2.3.1.pom (6.0 kB at 331 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/12/oss-parent-12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/12/oss-parent-12.pom (23 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.3.1/jackson-databind-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.3.1/jackson-databind-2.3.1.pom (5.9 kB at 296 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.0/jackson-annotations-2.3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.0/jackson-annotations-2.3.0.pom (1.3 kB at 72 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-json-provider/2.3.1/jackson-jaxrs-json-provider-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-json-provider/2.3.1/jackson-jaxrs-json-provider-2.3.1.pom (3.2 kB at 170 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-providers/2.3.1/jackson-jaxrs-providers-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-providers/2.3.1/jackson-jaxrs-providers-2.3.1.pom (3.8 kB at 221 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-base/2.3.1/jackson-jaxrs-base-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-base/2.3.1/jackson-jaxrs-base-2.3.1.pom (1.9 kB at 107 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-jaxb-annotations/2.3.1/jackson-module-jaxb-annotations-2.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-jaxb-annotations/2.3.1/jackson-module-jaxb-annotations-2.3.1.pom (4.5 kB at 237 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/inject/javax.inject/1/javax.inject-1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/inject/javax.inject/1/javax.inject-1.pom (612 B at 34 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/zapper/spice-zapper/1.3/spice-zapper-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/zapper/spice-zapper/1.3/spice-zapper-1.3.pom (4.6 kB at 255 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-proto/1.9/hawtbuf-proto-1.9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-proto/1.9/hawtbuf-proto-1.9.pom (4.5 kB at 248 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-project/1.9/hawtbuf-project-1.9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-project/1.9/hawtbuf-project-1.9.pom (11 kB at 535 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/fusesource-pom/1.9/fusesource-pom-1.9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/fusesource-pom/1.9/fusesource-pom-1.9.pom (15 kB at 740 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf/1.9/hawtbuf-1.9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf/1.9/hawtbuf-1.9.pom (2.6 kB at 144 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.pom (1.0 kB at 57 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.0.1/plexus-3.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.0.1/plexus-3.0.1.pom (19 kB at 886 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.pom (1.4 kB at 75 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether/1.13.1/aether-1.13.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether/1.13.1/aether-1.13.1.pom (10 kB at 563 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.1.2/logback-core-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.1.2/logback-core-1.1.2.pom (5.0 kB at 228 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-parent/1.1.2/logback-parent-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-parent/1.1.2/logback-parent-1.1.2.pom (15 kB at 784 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.1.2/logback-classic-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.1.2/logback-classic-1.1.2.pom (12 kB at 625 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plugins/nexus-staging-maven-plugin/1.6.8/nexus-staging-maven-plugin-1.6.8.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-common/1.6.8/nexus-common-1.6.8.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.7/plexus-cipher-1.7.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.4/plexus-sec-dispatcher-1.4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/14.0.1/guava-14.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/maven/nexus-common/1.6.8/nexus-common-1.6.8.jar (16 kB at 326 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-client-core/2.14.3-02/nexus-client-core-2.14.3-02.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.4/plexus-sec-dispatcher-1.4.jar (28 kB at 470 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-restlet1x-model/2.14.3-02/nexus-restlet1x-model-2.14.3-02.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plugins/nexus-staging-maven-plugin/1.6.8/nexus-staging-maven-plugin-1.6.8.jar (251 kB at 4.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.4/maven-model-3.0.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.7/plexus-cipher-1.7.jar (13 kB at 205 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.7/slf4j-api-1.7.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.7/slf4j-api-1.7.7.jar (29 kB at 329 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/2.0.1/jsr305-2.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/nexus-client-core/2.14.3-02/nexus-client-core-2.14.3-02.jar (216 kB at 2.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/intellij/annotations/9.0.4/annotations-9.0.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/nexus/plugins/nexus-restlet1x-model/2.14.3-02/nexus-restlet1x-model-2.14.3-02.jar (163 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0.4/maven-model-3.0.4.jar (164 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream/1.4.7/xstream-1.4.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/2.0.1/jsr305-2.0.1.jar (32 kB at 282 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xmlpull/xmlpull/1.1.3.1/xmlpull-1.1.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/intellij/annotations/9.0.4/annotations-9.0.4.jar (10.0 kB at 82 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xpp3/xpp3_min/1.1.4c/xpp3_min-1.1.4c.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xmlpull/xmlpull/1.1.3.1/xmlpull-1.1.3.1.jar (7.2 kB at 54 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/joda-time/joda-time/2.2/joda-time-2.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.4/commons-io-2.4.jar (185 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-beanutils/commons-beanutils-core/1.8.3/commons-beanutils-core-1.8.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xpp3/xpp3_min/1.1.4c/xpp3_min-1.1.4c.jar (25 kB at 164 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-client/1.7/siesta-client-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-client/1.7/siesta-client-1.7.jar (20 kB at 116 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-common/1.7/siesta-common-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/xstream/xstream/1.4.7/xstream-1.4.7.jar (532 kB at 3.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/ws/rs/jsr311-api/1.1.1/jsr311-api-1.1.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-beanutils/commons-beanutils-core/1.8.3/commons-beanutils-core-1.8.3.jar (207 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-core/1.17.1/jersey-core-1.17.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-common/1.7/siesta-common-1.7.jar (11 kB at 55 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/joda-time/joda-time/2.2/joda-time-2.2.jar (574 kB at 2.9 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-client/1.17.1/jersey-client-1.17.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/ws/rs/jsr311-api/1.1.1/jsr311-api-1.1.1.jar (46 kB at 234 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-apache-client4/1.17.1/jersey-apache-client4-1.17.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/contribs/jersey-apache-client4/1.17.1/jersey-apache-client4-1.17.1.jar (16 kB at 74 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-jackson/1.7/siesta-jackson-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar (64 kB at 291 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.1/jackson-annotations-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-client/1.17.1/jersey-client-1.17.1.jar (131 kB at 592 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.3.1/jackson-core-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/14.0.1/guava-14.0.1.jar (2.2 MB at 9.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.3.1/jackson-databind-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/sun/jersey/jersey-core/1.17.1/jersey-core-1.17.1.jar (467 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-json-provider/2.3.1/jackson-jaxrs-json-provider-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/siesta/siesta-jackson/1.7/siesta-jackson-1.7.jar (6.3 kB at 27 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-base/2.3.1/jackson-jaxrs-base-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-annotations/2.3.1/jackson-annotations-2.3.1.jar (37 kB at 152 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-jaxb-annotations/2.3.1/jackson-module-jaxb-annotations-2.3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-json-provider/2.3.1/jackson-jaxrs-json-provider-2.3.1.jar (16 kB at 66 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.3.5/httpclient-4.3.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.3.1/jackson-core-2.3.1.jar (198 kB at 786 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.6/commons-codec-1.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jaxrs/jackson-jaxrs-base/2.3.1/jackson-jaxrs-base-2.3.1.jar (28 kB at 108 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.3.2/httpcore-4.3.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/module/jackson-module-jaxb-annotations/2.3.1/jackson-module-jaxb-annotations-2.3.1.jar (32 kB at 118 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.7.7/jcl-over-slf4j-1.7.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-databind/2.3.1/jackson-databind-2.3.1.jar (914 kB at 3.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/inject/javax.inject/1/javax.inject-1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.6/commons-codec-1.6.jar (233 kB at 820 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/zapper/spice-zapper/1.3/spice-zapper-1.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.3.2/httpcore-4.3.2.jar (282 kB at 957 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-proto/1.9/hawtbuf-proto-1.9.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.7.7/jcl-over-slf4j-1.7.7.jar (17 kB at 56 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf/1.9/hawtbuf-1.9.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/inject/javax.inject/1/javax.inject-1.jar (2.5 kB at 8.4 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.8/plexus-utils-3.0.8.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.3.5/httpclient-4.3.5.jar (591 kB at 1.9 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/zapper/spice-zapper/1.3/spice-zapper-1.3.jar (121 kB at 392 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf/1.9/hawtbuf-1.9.jar (50 kB at 159 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.1.2/logback-core-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/fusesource/hawtbuf/hawtbuf-proto/1.9/hawtbuf-proto-1.9.jar (27 kB at 84 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.1.2/logback-classic-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.8/plexus-utils-3.0.8.jar (232 kB at 705 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.15/plexus-interpolation-1.15.jar (60 kB at 181 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.13.1/aether-api-1.13.1.jar (90 kB at 265 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-core/1.1.2/logback-core-1.1.2.jar (428 kB at 1.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/ch/qos/logback/logback-classic/1.1.2/logback-classic-1.1.2.jar (271 kB at 761 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-dependencies/0.18.0/google-cloud-shared-dependencies-0.18.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-dependencies/0.18.0/google-cloud-shared-dependencies-0.18.0.pom (9.9 kB at 494 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-config/0.9.4/google-cloud-shared-config-0.9.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-shared-config/0.9.4/google-cloud-shared-config-0.9.4.pom (32 kB at 1.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-bom/1.34.1/grpc-bom-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-bom/1.34.1/grpc-bom-1.34.1.pom (4.6 kB at 241 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax-bom/1.60.1/gax-bom-1.60.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax-bom/1.60.1/gax-bom-1.60.1.pom (2.7 kB at 140 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-bom/30.1-android/guava-bom-30.1-android.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-bom/30.1-android/guava-bom-30.1-android.pom (1.5 kB at 85 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/oss/oss-parent/9/oss-parent-9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/oss/oss-parent/9/oss-parent-9.pom (6.6 kB at 365 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-bom/3.14.0/protobuf-bom-3.14.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-bom/3.14.0/protobuf-bom-3.14.0.pom (3.5 kB at 84 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-core-bom/1.94.0/google-cloud-core-bom-1.94.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/cloud/google-cloud-core-bom/1.94.0/google-cloud-core-bom-1.94.0.pom (3.0 kB at 157 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-bom/0.22.2/google-auth-library-bom-0.22.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-bom/0.22.2/google-auth-library-bom-0.22.2.pom (4.8 kB at 266 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-bom/1.38.0/google-http-client-bom-1.38.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-bom/1.38.0/google-http-client-bom-1.38.0.pom (7.1 kB at 373 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api-client/google-api-client-bom/1.31.1/google-api-client-bom-1.31.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api-client/google-api-client-bom/1.31.1/google-api-client-bom-1.31.1.pom (7.0 kB at 367 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-bom/2.12.1/jackson-bom-2.12.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-bom/2.12.1/jackson-bom-2.12.1.pom (15 kB at 766 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-parent/2.12/jackson-parent-2.12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-parent/2.12/jackson-parent-2.12.pom (7.5 kB at 396 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/41/oss-parent-41.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/oss-parent/41/oss-parent-41.pom (23 kB at 1.2 MB/s)
[WARNING] 
[WARNING] Some problems were encountered while building the effective model for com.google.cloud:google-cloud-video-intelligence-bom:pom:1.5.9
[WARNING] 'build.plugins.plugin.version' for org.apache.maven.plugins:maven-checkstyle-plugin is missing. @ line 124, column 15
[WARNING] 
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING] 
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[WARNING] 
[INFO] Inspecting build with total of 13 modules...
[INFO] Installing Nexus Staging features:
[INFO]   ... total of 13 executions of maven-deploy-plugin replaced with nexus-staging-maven-plugin
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] Google Cloud Video Intelligence Parent                             [pom]
[INFO] proto-google-cloud-video-intelligence-v1p3beta1                    [jar]
[INFO] proto-google-cloud-video-intelligence-v1beta2                      [jar]
[INFO] proto-google-cloud-video-intelligence-v1p1beta1                    [jar]
[INFO] proto-google-cloud-video-intelligence-v1                           [jar]
[INFO] proto-google-cloud-video-intelligence-v1p2beta1                    [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p1beta1                     [jar]
[INFO] grpc-google-cloud-video-intelligence-v1beta2                       [jar]
[INFO] grpc-google-cloud-video-intelligence-v1                            [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p2beta1                     [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p3beta1                     [jar]
[INFO] Google Cloud Video Intelligence                                    [jar]
[INFO] Google Cloud video-intelligence BOM                                [pom]
[INFO] 
[INFO] Using the MultiThreadedBuilder implementation with a thread count of 4
[INFO] 
[INFO] 
[INFO] --------< com.google.cloud:google-cloud-video-intelligence-bom >--------
[INFO] Building Google Cloud video-intelligence BOM 1.5.9                [1/13]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] ------< com.google.cloud:google-cloud-video-intelligence-parent >-------
[INFO] Building Google Cloud Video Intelligence Parent 1.5.9             [2/13]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-enforcer-plugin/3.0.0-M3/maven-enforcer-plugin-3.0.0-M3.pom
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/maven-metadata.xml
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-enforcer-plugin/3.0.0-M3/maven-enforcer-plugin-3.0.0-M3.pom (7.3 kB at 367 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/maven-metadata.xml (1.1 kB at 65 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer/3.0.0-M3/enforcer-3.0.0-M3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer/3.0.0-M3/enforcer-3.0.0-M3.pom (7.8 kB at 411 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/33/maven-parent-33.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/33/maven-parent-33.pom (44 kB at 2.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/21/apache-21.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/21/apache-21.pom (17 kB at 900 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-enforcer-plugin/3.0.0-M3/maven-enforcer-plugin-3.0.0-M3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-enforcer-plugin/3.0.0-M3/maven-enforcer-plugin-3.0.0-M3.jar (27 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/3.1.2/maven-checkstyle-plugin-3.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/3.1.2/maven-checkstyle-plugin-3.1.2.pom (15 kB at 841 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/34/maven-plugins-34.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/34/maven-plugins-34.pom (11 kB at 629 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/34/maven-parent-34.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/34/maven-parent-34.pom (43 kB at 2.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/23/apache-23.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/23/apache-23.pom (18 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/3.1.2/maven-checkstyle-plugin-3.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-checkstyle-plugin/3.1.2/maven-checkstyle-plugin-3.1.2.jar (112 kB at 5.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/exec-maven-plugin/3.0.0/exec-maven-plugin-3.0.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/exec-maven-plugin/3.0.0/exec-maven-plugin-3.0.0.pom (14 kB at 798 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/mojo-parent/50/mojo-parent-50.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/mojo-parent/50/mojo-parent-50.pom (34 kB at 1.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/exec-maven-plugin/3.0.0/exec-maven-plugin-3.0.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/exec-maven-plugin/3.0.0/exec-maven-plugin-3.0.0.jar (68 kB at 3.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-failsafe-plugin/3.0.0-M4/maven-failsafe-plugin-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-failsafe-plugin/3.0.0-M4/maven-failsafe-plugin-3.0.0-M4.pom (15 kB at 859 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/3.0.0-M4/surefire-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/3.0.0-M4/surefire-3.0.0-M4.pom (27 kB at 1.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-failsafe-plugin/3.0.0-M4/maven-failsafe-plugin-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-failsafe-plugin/3.0.0-M4/maven-failsafe-plugin-3.0.0-M4.jar (302 kB at 11 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/3.2.0/maven-jar-plugin-3.2.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/3.2.0/maven-jar-plugin-3.2.0.pom (7.3 kB at 363 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/33/maven-plugins-33.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-plugins/33/maven-plugins-33.pom (11 kB at 629 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/3.2.0/maven-jar-plugin-3.2.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-jar-plugin/3.2.0/maven-jar-plugin-3.2.0.jar (29 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/jacoco-maven-plugin/0.8.6/jacoco-maven-plugin-0.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/jacoco-maven-plugin/0.8.6/jacoco-maven-plugin-0.8.6.pom (4.4 kB at 256 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.build/0.8.6/org.jacoco.build-0.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.build/0.8.6/org.jacoco.build-0.8.6.pom (42 kB at 2.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/jacoco-maven-plugin/0.8.6/jacoco-maven-plugin-0.8.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/jacoco-maven-plugin/0.8.6/jacoco-maven-plugin-0.8.6.jar (53 kB at 2.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/clirr-maven-plugin/2.8/clirr-maven-plugin-2.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/clirr-maven-plugin/2.8/clirr-maven-plugin-2.8.pom (8.0 kB at 444 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/mojo-parent/38/mojo-parent-38.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/mojo-parent/38/mojo-parent-38.pom (33 kB at 1.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/clirr-maven-plugin/2.8/clirr-maven-plugin-2.8.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/clirr-maven-plugin/2.8/clirr-maven-plugin-2.8.jar (75 kB at 3.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/build-helper-maven-plugin/3.2.0/build-helper-maven-plugin-3.2.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/build-helper-maven-plugin/3.2.0/build-helper-maven-plugin-3.2.0.pom (7.3 kB at 404 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/build-helper-maven-plugin/3.2.0/build-helper-maven-plugin-3.2.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/build-helper-maven-plugin/3.2.0/build-helper-maven-plugin-3.2.0.jar (69 kB at 3.5 MB/s)
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] *****************************************************************
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in Google Cloud Video Intelligence Parent:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in Google Cloud video-intelligence BOM:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] 
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-bom ---
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-parent ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/extra-enforcer-rules/1.3/extra-enforcer-rules-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/extra-enforcer-rules/1.3/extra-enforcer-rules-1.3.pom (8.4 kB at 301 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-api/3.0.0-M3/enforcer-api-3.0.0-M3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-api/3.0.0-M3/enforcer-api-3.0.0-M3.pom (2.8 kB at 157 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0/maven-plugin-api-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0/maven-plugin-api-3.0.pom (2.3 kB at 127 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0/maven-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0/maven-3.0.pom (22 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0/maven-model-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0/maven-model-3.0.pom (3.9 kB at 205 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.3.0/plexus-utils-3.3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.3.0/plexus-utils-3.3.0.pom (5.2 kB at 305 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/5.1/plexus-5.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/5.1/plexus-5.1.pom (23 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0/maven-artifact-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0/maven-artifact-3.0.pom (1.9 kB at 66 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/1.4.2/sisu-inject-plexus-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/1.4.2/sisu-inject-plexus-1.4.2.pom (5.4 kB at 283 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-plexus/1.4.2/guice-plexus-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-plexus/1.4.2/guice-plexus-1.4.2.pom (3.1 kB at 174 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-bean/1.4.2/guice-bean-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-bean/1.4.2/guice-bean-1.4.2.pom (2.6 kB at 137 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject/1.4.2/sisu-inject-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject/1.4.2/sisu-inject-1.4.2.pom (1.2 kB at 73 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-parent/1.4.2/sisu-parent-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-parent/1.4.2/sisu-parent-1.4.2.pom (7.8 kB at 409 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/6/forge-parent-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/6/forge-parent-6.pom (11 kB at 512 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7.1/plexus-component-annotations-1.7.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7.1/plexus-component-annotations-1.7.1.pom (770 B at 43 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.7.1/plexus-containers-1.7.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.7.1/plexus-containers-1.7.1.pom (5.0 kB at 265 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/4.0/plexus-4.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/4.0/plexus-4.0.pom (22 kB at 860 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.3/plexus-classworlds-2.2.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.3/plexus-classworlds-2.2.3.pom (4.0 kB at 210 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/2.0.6/plexus-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/2.0.6/plexus-2.0.6.pom (17 kB at 931 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/1.4.2/sisu-inject-bean-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/1.4.2/sisu-inject-bean-1.4.2.pom (5.5 kB at 303 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/2.1.7/sisu-guice-2.1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/2.1.7/sisu-guice-2.1.7.pom (11 kB at 651 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.11/junit-4.11.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.11/junit-4.11.pom (2.3 kB at 138 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.pom (766 B at 45 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-parent/1.3/hamcrest-parent-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-parent/1.3/hamcrest-parent-1.3.pom (2.0 kB at 116 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0/maven-core-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0/maven-core-3.0.pom (6.6 kB at 390 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0/maven-settings-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0/maven-settings-3.0.pom (1.9 kB at 104 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0/maven-settings-builder-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0/maven-settings-builder-3.0.pom (2.2 kB at 123 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.14/plexus-interpolation-1.14.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.14/plexus-interpolation-1.14.pom (910 B at 51 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.18/plexus-components-1.1.18.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.18/plexus-components-1.1.18.pom (5.4 kB at 298 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.3/plexus-sec-dispatcher-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.3/plexus-sec-dispatcher-1.3.pom (3.0 kB at 174 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.4/plexus-cipher-1.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.4/plexus-cipher-1.4.pom (2.1 kB at 121 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0/maven-repository-metadata-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0/maven-repository-metadata-3.0.pom (1.9 kB at 113 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0/maven-model-builder-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0/maven-model-builder-3.0.pom (2.2 kB at 132 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0/maven-aether-provider-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0/maven-aether-provider-3.0.pom (2.5 kB at 130 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.7/aether-api-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.7/aether-api-1.7.pom (1.7 kB at 93 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-parent/1.7/aether-parent-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-parent/1.7/aether-parent-1.7.pom (7.7 kB at 386 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.7/aether-util-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.7/aether-util-1.7.pom (2.1 kB at 86 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.7/aether-impl-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.7/aether-impl-1.7.pom (3.7 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.7/aether-spi-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.7/aether-spi-1.7.pom (1.7 kB at 87 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-dependency-tree/2.2/maven-dependency-tree-2.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-dependency-tree/2.2/maven-dependency-tree-2.2.pom (7.3 kB at 363 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/20/maven-shared-components-20.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/20/maven-shared-components-20.pom (5.1 kB at 255 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/24/maven-parent-24.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/24/maven-parent-24.pom (37 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/14/apache-14.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/14/apache-14.pom (15 kB at 773 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.12/commons-codec-1.12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.12/commons-codec-1.12.pom (14 kB at 791 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/47/commons-parent-47.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/47/commons-parent-47.pom (78 kB at 3.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/19/apache-19.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/19/apache-19.pom (15 kB at 860 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.1.0/maven-common-artifact-filters-3.1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.1.0/maven-common-artifact-filters-3.1.0.pom (5.3 kB at 278 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/33/maven-shared-components-33.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/33/maven-shared-components-33.pom (5.1 kB at 255 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.1.0/maven-shared-utils-3.1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.1.0/maven-shared-utils-3.1.0.pom (5.0 kB at 262 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/30/maven-shared-components-30.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/30/maven-shared-components-30.pom (4.6 kB at 270 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/30/maven-parent-30.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/30/maven-parent-30.pom (41 kB at 2.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/18/apache-18.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/18/apache-18.pom (16 kB at 922 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.5/commons-io-2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.5/commons-io-2.5.pom (13 kB at 738 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/39/commons-parent-39.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/39/commons-parent-39.pom (62 kB at 3.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/16/apache-16.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/16/apache-16.pom (15 kB at 770 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-rules/3.0.0-M3/enforcer-rules-3.0.0-M3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-rules/3.0.0-M3/enforcer-rules-3.0.0-M3.pom (4.1 kB at 243 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.8.1/commons-lang3-3.8.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.8.1/commons-lang3-3.8.1.pom (28 kB at 1.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/beanshell/bsh/2.0b4/bsh-2.0b4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/beanshell/bsh/2.0b4/bsh-2.0b4.pom (1.2 kB at 70 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/beanshell/beanshell/2.0b4/beanshell-2.0b4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/beanshell/beanshell/2.0b4/beanshell-2.0b4.pom (1.4 kB at 83 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.pom (2.8 kB at 122 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver/1.4.1/maven-resolver-1.4.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver/1.4.1/maven-resolver-1.4.1.pom (18 kB at 957 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.pom (2.6 kB at 164 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-compat/3.0/maven-compat-3.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-compat/3.0/maven-compat-3.0.pom (4.0 kB at 223 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/1.0-beta-6/wagon-provider-api-1.0-beta-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/1.0-beta-6/wagon-provider-api-1.0-beta-6.pom (1.8 kB at 88 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon/1.0-beta-6/wagon-1.0-beta-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon/1.0-beta-6/wagon-1.0-beta-6.pom (12 kB at 619 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/extra-enforcer-rules/1.3/extra-enforcer-rules-1.3.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-dependency-tree/2.2/maven-dependency-tree-2.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.11/junit-4.11.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.0-alpha-9/plexus-container-default-1.0-alpha-9.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/extra-enforcer-rules/1.3/extra-enforcer-rules-1.3.jar (52 kB at 2.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.12/commons-codec-1.12.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-core/1.3/hamcrest-core-1.3.jar (45 kB at 1.9 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.1.0/maven-common-artifact-filters-3.1.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-dependency-tree/2.2/maven-dependency-tree-2.2.jar (64 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.1.0/maven-shared-utils-3.1.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-container-default/1.0-alpha-9/plexus-container-default-1.0-alpha-9.jar (195 kB at 5.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.5/commons-io-2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.1.0/maven-common-artifact-filters-3.1.0.jar (61 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0/maven-artifact-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.12/commons-codec-1.12.jar (340 kB at 6.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0/maven-plugin-api-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.11/junit-4.11.jar (245 kB at 4.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0/maven-model-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.1.0/maven-shared-utils-3.1.0.jar (164 kB at 2.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/1.4.2/sisu-inject-plexus-1.4.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.5/commons-io-2.5.jar (209 kB at 3.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/1.4.2/sisu-inject-bean-1.4.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.0/maven-artifact-3.0.jar (52 kB at 775 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/2.1.7/sisu-guice-2.1.7-noaop.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.0/maven-plugin-api-3.0.jar (49 kB at 699 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0/maven-core-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.0/maven-model-3.0.jar (165 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0/maven-settings-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-bean/1.4.2/sisu-inject-bean-1.4.2.jar (153 kB at 1.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0/maven-settings-builder-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-inject-plexus/1.4.2/sisu-inject-plexus-1.4.2.jar (202 kB at 2.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0/maven-repository-metadata-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.0/maven-settings-3.0.jar (47 kB at 458 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0/maven-model-builder-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.0/maven-settings-builder-3.0.jar (38 kB at 360 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0/maven-aether-provider-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.0/maven-core-3.0.jar (527 kB at 5.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.7/aether-impl-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.0/maven-repository-metadata-3.0.jar (30 kB at 259 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.7/aether-spi-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/2.1.7/sisu-guice-2.1.7-noaop.jar (472 kB at 3.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.7/aether-api-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.0/maven-aether-provider-3.0.jar (51 kB at 406 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.7/aether-util-1.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.0/maven-model-builder-3.0.jar (148 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.14/plexus-interpolation-1.14.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-impl/1.7/aether-impl-1.7.jar (106 kB at 805 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.3/plexus-classworlds-2.2.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-spi/1.7/aether-spi-1.7.jar (14 kB at 101 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7.1/plexus-component-annotations-1.7.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-api/1.7/aether-api-1.7.jar (74 kB at 501 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.3/plexus-sec-dispatcher-1.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/aether/aether-util/1.7/aether-util-1.7.jar (108 kB at 724 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.4/plexus-cipher-1.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.14/plexus-interpolation-1.14.jar (61 kB at 402 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7.1/plexus-component-annotations-1.7.1.jar (4.3 kB at 28 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-api/3.0.0-M3/enforcer-api-3.0.0-M3.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.3.0/plexus-utils-3.3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.2.3/plexus-classworlds-2.2.3.jar (46 kB at 299 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-rules/3.0.0-M3/enforcer-rules-3.0.0-M3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-sec-dispatcher/1.3/plexus-sec-dispatcher-1.3.jar (29 kB at 173 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.8.1/commons-lang3-3.8.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-cipher/1.4/plexus-cipher-1.4.jar (13 kB at 81 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-api/3.0.0-M3/enforcer-api-3.0.0-M3.jar (12 kB at 69 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/beanshell/bsh/2.0b4/bsh-2.0b4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/enforcer/enforcer-rules/3.0.0-M3/enforcer-rules-3.0.0-M3.jar (107 kB at 598 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.3.0/plexus-utils-3.3.0.jar (263 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-compat/3.0/maven-compat-3.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.8.1/commons-lang3-3.8.1.jar (502 kB at 2.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/1.0-beta-6/wagon-provider-api-1.0-beta-6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.jar (168 kB at 829 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.jar (149 kB at 727 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/beanshell/bsh/2.0b4/bsh-2.0b4.jar (282 kB at 1.3 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/1.0-beta-6/wagon-provider-api-1.0-beta-6.jar (53 kB at 246 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-compat/3.0/maven-compat-3.0.jar (285 kB at 1.3 MB/s)
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-bom ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-parent ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.4/plexus-utils-2.0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.4/plexus-utils-2.0.4.pom (3.3 kB at 152 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.5.4/plexus-component-annotations-1.5.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.5.4/plexus-component-annotations-1.5.4.pom (815 B at 45 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.5.4/plexus-containers-1.5.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.5.4/plexus-containers-1.5.4.pom (4.2 kB at 236 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/2.0.5/plexus-2.0.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/2.0.5/plexus-2.0.5.pom (17 kB at 826 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.pom (3.3 kB at 196 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.5/plexus-utils-1.5.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.5/plexus-utils-1.5.5.pom (5.1 kB at 303 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.22/plexus-utils-3.0.22.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.22/plexus-utils-3.0.22.pom (3.8 kB at 225 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.3.1/plexus-3.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/3.3.1/plexus-3.3.1.pom (20 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.13/junit-4.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.13/junit-4.13.pom (25 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-impl/2.1/maven-reporting-impl-2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-impl/2.1/maven-reporting-impl-2.1.pom (4.5 kB at 251 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.10/maven-project-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.10/maven-project-2.0.10.pom (2.8 kB at 158 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.0.10/maven-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.0.10/maven-2.0.10.pom (24 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.10/maven-settings-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.0.10/maven-settings-2.0.10.pom (2.2 kB at 124 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.10/maven-model-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.0.10/maven-model-2.0.10.pom (3.3 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.1/plexus-interpolation-1.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.1/plexus-interpolation-1.1.pom (1.4 kB at 80 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.10/maven-profile-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.10/maven-profile-2.0.10.pom (2.1 kB at 123 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.10/maven-artifact-manager-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.10/maven-artifact-manager-2.0.10.pom (2.7 kB at 150 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.10/maven-repository-metadata-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.0.10/maven-repository-metadata-2.0.10.pom (2.3 kB at 136 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.10/maven-artifact-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.0.10/maven-artifact-2.0.10.pom (1.6 kB at 101 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.10/maven-plugin-registry-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.10/maven-plugin-registry-2.0.10.pom (2.0 kB at 106 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.10/maven-plugin-api-2.0.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.0.10/maven-plugin-api-2.0.10.pom (1.5 kB at 88 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.1.2/doxia-sink-api-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.1.2/doxia-sink-api-1.1.2.pom (1.6 kB at 88 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.1.2/doxia-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia/1.1.2/doxia-1.1.2.pom (18 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1.2/doxia-logging-api-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1.2/doxia-logging-api-1.1.2.pom (1.6 kB at 93 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-core/1.1.2/doxia-core-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-core/1.1.2/doxia-core-1.1.2.pom (3.7 kB at 219 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.12/plexus-utils-1.5.12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.5.12/plexus-utils-1.5.12.pom (5.6 kB at 313 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xerces/xercesImpl/2.8.1/xercesImpl-2.8.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xerces/xercesImpl/2.8.1/xercesImpl-2.8.1.pom (2.2 kB at 130 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xml-apis/xml-apis/1.3.03/xml-apis-1.3.03.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xml-apis/xml-apis/1.3.03/xml-apis-1.3.03.pom (738 B at 43 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/1/apache-1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/1/apache-1.pom (3.4 kB at 189 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.4/commons-lang-2.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.4/commons-lang-2.4.pom (14 kB at 822 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.pom (7.8 kB at 370 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.2/commons-codec-1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.2/commons-codec-1.2.pom (3.8 kB at 225 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-site-renderer/1.1.2/doxia-site-renderer-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-site-renderer/1.1.2/doxia-site-renderer-1.1.2.pom (6.1 kB at 322 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sitetools/1.1.2/doxia-sitetools-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sitetools/1.1.2/doxia-sitetools-1.1.2.pom (15 kB at 849 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-decoration-model/1.1.2/doxia-decoration-model-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-decoration-model/1.1.2/doxia-decoration-model-1.1.2.pom (3.0 kB at 165 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-xhtml/1.1.2/doxia-module-xhtml-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-xhtml/1.1.2/doxia-module-xhtml-1.1.2.pom (1.6 kB at 89 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-modules/1.1.2/doxia-modules-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-modules/1.1.2/doxia-modules-1.1.2.pom (2.4 kB at 135 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-fml/1.1.2/doxia-module-fml-1.1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-fml/1.1.2/doxia-module-fml-1.1.2.pom (5.5 kB at 323 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.pom (12 kB at 689 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6.pom (3.5 kB at 167 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.core/0.8.6/org.jacoco.core-0.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.core/0.8.6/org.jacoco.core-0.8.6.pom (2.1 kB at 116 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/8.0.1/asm-8.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/8.0.1/asm-8.0.1.pom (2.9 kB at 164 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/ow2/1.5/ow2-1.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/ow2/1.5/ow2-1.5.pom (11 kB at 562 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-commons/8.0.1/asm-commons-8.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-commons/8.0.1/asm-commons-8.0.1.pom (3.7 kB at 194 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-tree/8.0.1/asm-tree-8.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-tree/8.0.1/asm-tree-8.0.1.pom (3.1 kB at 174 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-analysis/8.0.1/asm-analysis-8.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-analysis/8.0.1/asm-analysis-8.0.1.pom (3.2 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.report/0.8.6/org.jacoco.report-0.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.report/0.8.6/org.jacoco.report-0.8.6.pom (1.9 kB at 99 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.22/plexus-utils-3.0.22.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.13/junit-4.13.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-impl/2.1/maven-reporting-impl-2.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.2/maven-artifact-manager-2.0.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.10/maven-project-2.0.10.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.0.2/maven-artifact-manager-2.0.2.jar (49 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.10/maven-profile-2.0.10.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-impl/2.1/maven-reporting-impl-2.1.jar (17 kB at 488 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.10/maven-plugin-registry-2.0.10.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.22/plexus-utils-3.0.22.jar (245 kB at 6.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-core/1.1.2/doxia-core-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.0.10/maven-project-2.0.10.jar (123 kB at 3.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1.2/doxia-logging-api-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.13/junit-4.13.jar (382 kB at 8.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/xerces/xercesImpl/2.8.1/xercesImpl-2.8.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.0.10/maven-profile-2.0.10.jar (37 kB at 785 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.4/commons-lang-2.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.0.10/maven-plugin-registry-2.0.10.jar (30 kB at 707 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-logging-api/1.1.2/doxia-logging-api-1.1.2.jar (11 kB at 227 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.2/commons-codec-1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-core/1.1.2/doxia-core-1.1.2.jar (158 kB at 2.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-site-renderer/1.1.2/doxia-site-renderer-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.2/commons-codec-1.2.jar (30 kB at 442 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-decoration-model/1.1.2/doxia-decoration-model-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar (305 kB at 4.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-xhtml/1.1.2/doxia-module-xhtml-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-site-renderer/1.1.2/doxia-site-renderer-1.1.2.jar (50 kB at 631 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-fml/1.1.2/doxia-module-fml-1.1.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.4/commons-lang-2.4.jar (262 kB at 3.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-xhtml/1.1.2/doxia-module-xhtml-1.1.2.jar (15 kB at 156 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/xerces/xercesImpl/2.8.1/xercesImpl-2.8.1.jar (1.2 MB at 13 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.core/0.8.6/org.jacoco.core-0.8.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-module-fml/1.1.2/doxia-module-fml-1.1.2.jar (37 kB at 378 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/8.0.1/asm-8.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-decoration-model/1.1.2/doxia-decoration-model-1.1.2.jar (52 kB at 523 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-commons/8.0.1/asm-commons-8.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-commons/8.0.1/asm-commons-8.0.1.jar (72 kB at 587 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-analysis/8.0.1/asm-analysis-8.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/8.0.1/asm-8.0.1.jar (122 kB at 990 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-tree/8.0.1/asm-tree-8.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar (292 kB at 2.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.report/0.8.6/org.jacoco.report-0.8.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.core/0.8.6/org.jacoco.core-0.8.6.jar (199 kB at 1.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar (588 kB at 4.7 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-analysis/8.0.1/asm-analysis-8.0.1.jar (33 kB at 241 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jacoco/org.jacoco.report/0.8.6/org.jacoco.report-0.8.6.jar (129 kB at 883 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm-tree/8.0.1/asm-tree-8.0.1.jar (53 kB at 360 kB/s)
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/target/jacoco.exec
[INFO] 
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/target/jacoco.exec
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-parent ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.24/plexus-utils-3.0.24.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.24/plexus-utils-3.0.24.pom (4.1 kB at 243 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache-extras/beanshell/bsh/2.0b6/bsh-2.0b6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache-extras/beanshell/bsh/2.0b6/bsh-2.0b6.pom (5.0 kB at 277 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.0.0/file-management-3.0.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.0.0/file-management-3.0.0.pom (4.7 kB at 293 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/22/maven-shared-components-22.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/22/maven-shared-components-22.pom (5.1 kB at 320 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/27/maven-parent-27.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/27/maven-parent-27.pom (41 kB at 2.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/17/apache-17.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/17/apache-17.pom (16 kB at 944 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-io/3.0.0/maven-shared-io-3.0.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-io/3.0.0/maven-shared-io-3.0.0.pom (4.2 kB at 245 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.4.2/plexus-utils-1.4.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.4.2/plexus-utils-1.4.2.pom (2.0 kB at 122 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/2.10/wagon-provider-api-2.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/2.10/wagon-provider-api-2.10.pom (1.7 kB at 102 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon/2.10/wagon-2.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon/2.10/wagon-2.10.pom (21 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/26/maven-parent-26.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/26/maven-parent-26.pom (40 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.15/plexus-utils-3.0.15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.15/plexus-utils-3.0.15.pom (3.1 kB at 197 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.0.0/maven-shared-utils-3.0.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.0.0/maven-shared-utils-3.0.0.pom (5.6 kB at 266 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/21/maven-shared-components-21.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/21/maven-shared-components-21.pom (5.1 kB at 269 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/25/maven-parent-25.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/25/maven-parent-25.pom (37 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/15/apache-15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/15/apache-15.pom (15 kB at 896 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.24/plexus-utils-3.0.24.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache-extras/beanshell/bsh/2.0b6/bsh-2.0b6.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.0.0/file-management-3.0.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-io/3.0.0/maven-shared-io-3.0.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/2.10/wagon-provider-api-2.10.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/wagon/wagon-provider-api/2.10/wagon-provider-api-2.10.jar (54 kB at 2.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.0.0/maven-shared-utils-3.0.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-io/3.0.0/maven-shared-io-3.0.0.jar (41 kB at 1.9 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.0.0/file-management-3.0.0.jar (35 kB at 1.5 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.24/plexus-utils-3.0.24.jar (247 kB at 8.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.0.0/maven-shared-utils-3.0.0.jar (155 kB at 3.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache-extras/beanshell/bsh/2.0b6/bsh-2.0b6.jar (389 kB at 8.1 MB/s)
[INFO] 
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence-parent ---
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence-bom ---
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence-parent ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ google-cloud-video-intelligence-parent ---
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ google-cloud-video-intelligence-bom ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.5.0/maven-archiver-3.5.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.5.0/maven-archiver-3.5.0.pom (4.5 kB at 235 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.2.1/maven-shared-utils-3.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.2.1/maven-shared-utils-3.2.1.pom (5.6 kB at 313 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.0/plexus-archiver-4.2.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.0/plexus-archiver-4.2.0.pom (4.8 kB at 284 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.2.0/plexus-io-3.2.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.2.0/plexus-io-3.2.0.pom (4.5 kB at 253 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.6/commons-io-2.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.6/commons-io-2.6.pom (14 kB at 792 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/42/commons-parent-42.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/42/commons-parent-42.pom (68 kB at 3.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.19/commons-compress-1.19.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.19/commons-compress-1.19.pom (18 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/48/commons-parent-48.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/48/commons-parent-48.pom (72 kB at 3.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.pom (15 kB at 808 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.8/xz-1.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.8/xz-1.8.pom (1.9 kB at 76 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.25/plexus-interpolation-1.25.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.25/plexus-interpolation-1.25.pom (2.6 kB at 156 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.1/plexus-archiver-4.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.1/plexus-archiver-4.2.1.pom (4.8 kB at 269 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.5.0/maven-archiver-3.5.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.1/plexus-archiver-4.2.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.2.1/maven-shared-utils-3.2.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.2.0/plexus-io-3.2.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.19/commons-compress-1.19.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.5.0/maven-archiver-3.5.0.jar (26 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.2.0/plexus-io-3.2.0.jar (76 kB at 3.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.8/xz-1.8.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/3.2.1/maven-shared-utils-3.2.1.jar (167 kB at 5.9 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.2.1/plexus-archiver-4.2.1.jar (196 kB at 6.3 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.jar (58 kB at 1.5 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.8/xz-1.8.jar (109 kB at 2.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.19/commons-compress-1.19.jar (615 kB at 9.0 MB/s)
[WARNING] JAR will be empty - no content was marked for inclusion!
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/target/google-cloud-video-intelligence-bom-1.5.9-tests.jar
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/target/google-cloud-video-intelligence-parent-1.5.9-tests.jar
[INFO] 
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ google-cloud-video-intelligence-parent ---
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ google-cloud-video-intelligence-bom ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M4/surefire-junit47-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M4/surefire-junit47-3.0.0-M4.pom (8.3 kB at 464 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/3.0.0-M4/surefire-providers-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/3.0.0-M4/surefire-providers-3.0.0-M4.pom (2.5 kB at 158 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M4/common-junit48-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M4/common-junit48-3.0.0-M4.pom (3.2 kB at 179 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M4/common-junit4-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M4/common-junit4-3.0.0-M4.pom (2.9 kB at 155 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M4/common-junit3-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M4/common-junit3-3.0.0-M4.pom (2.6 kB at 153 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M4/surefire-api-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M4/surefire-api-3.0.0-M4.pom (5.1 kB at 285 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M4/surefire-logger-api-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M4/surefire-logger-api-3.0.0-M4.pom (3.6 kB at 189 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M4/common-java5-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M4/common-java5-3.0.0-M4.pom (3.8 kB at 197 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M4/surefire-grouper-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M4/surefire-grouper-3.0.0-M4.pom (3.1 kB at 173 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M4/maven-surefire-common-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M4/maven-surefire-common-3.0.0-M4.pom (13 kB at 641 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M4/surefire-extensions-api-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M4/surefire-extensions-api-3.0.0-M4.pom (3.8 kB at 183 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M4/surefire-booter-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M4/surefire-booter-3.0.0-M4.pom (8.0 kB at 469 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/3.0-alpha-2/maven-toolchain-3.0-alpha-2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/3.0-alpha-2/maven-toolchain-3.0-alpha-2.pom (2.2 kB at 131 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0-alpha-2/maven-3.0-alpha-2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.0-alpha-2/maven-3.0-alpha-2.pom (21 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.11.0/maven-artifact-transfer-0.11.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.11.0/maven-artifact-transfer-0.11.0.pom (11 kB at 545 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.11/commons-codec-1.11.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.11/commons-codec-1.11.pom (14 kB at 776 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.3/plexus-java-1.0.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.3/plexus-java-1.0.3.pom (4.8 kB at 280 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/1.0.3/plexus-languages-1.0.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/1.0.3/plexus-languages-1.0.3.pom (4.2 kB at 248 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.0/asm-7.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.0/asm-7.0.pom (2.9 kB at 173 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M9/qdox-2.0-M9.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M9/qdox-2.0-M9.pom (16 kB at 880 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M4/surefire-junit47-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M4/common-junit4-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M4/common-junit3-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M4/common-java5-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M4/common-junit48-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M4/common-junit4-3.0.0-M4.jar (27 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M4/surefire-grouper-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M4/common-java5-3.0.0-M4.jar (33 kB at 1.4 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M4/common-junit48-3.0.0-M4.jar (21 kB at 846 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M4/surefire-junit47-3.0.0-M4.jar (92 kB at 3.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M4/surefire-logger-api-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M4/surefire-api-3.0.0-M4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M4/maven-surefire-common-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M4/common-junit3-3.0.0-M4.jar (12 kB at 384 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M4/surefire-extensions-api-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M4/surefire-grouper-3.0.0-M4.jar (40 kB at 954 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M4/surefire-booter-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M4/surefire-logger-api-3.0.0-M4.jar (14 kB at 324 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/3.0-alpha-2/maven-toolchain-3.0-alpha-2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M4/surefire-extensions-api-3.0.0-M4.jar (14 kB at 284 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.11.0/maven-artifact-transfer-0.11.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M4/surefire-api-3.0.0-M4.jar (343 kB at 6.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.11/commons-codec-1.11.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-toolchain/3.0-alpha-2/maven-toolchain-3.0-alpha-2.jar (36 kB at 573 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.3/plexus-java-1.0.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.11.0/maven-artifact-transfer-0.11.0.jar (128 kB at 1.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.0/asm-7.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M4/maven-surefire-common-3.0.0-M4.jar (804 kB at 10 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M4/surefire-booter-3.0.0-M4.jar (317 kB at 4.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M9/qdox-2.0-M9.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.1/plexus-utils-1.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.11/commons-codec-1.11.jar (335 kB at 3.9 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.3/plexus-java-1.0.3.jar (51 kB at 565 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.0/asm-7.0.jar (114 kB at 1.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/1.1/plexus-utils-1.1.jar (169 kB at 1.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/thoughtworks/qdox/qdox/2.0-M9/qdox-2.0-M9.jar (317 kB at 2.8 MB/s)
[INFO] Tests are skipped.
[INFO] Tests are skipped.
[INFO] 
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ google-cloud-video-intelligence-parent ---
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ google-cloud-video-intelligence-bom ---
[INFO] Tests are skipped.
[INFO] Tests are skipped.
[INFO] 
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ google-cloud-video-intelligence-parent >>>
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ google-cloud-video-intelligence-bom >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-parent ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-bom ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-parent ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/target/jacoco.exec
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/target/jacoco.exec
[INFO] 
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-bom ---
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-parent ---
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ google-cloud-video-intelligence-bom <<<
[INFO] 
[INFO] 
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ google-cloud-video-intelligence-parent <<<
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ google-cloud-video-intelligence-parent ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/net/sf/clirr/clirr-core/0.6/clirr-core-0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/net/sf/clirr/clirr-core/0.6/clirr-core-0.6.pom (3.8 kB at 190 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/bcel/bcel/6.0/bcel-6.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/bcel/bcel/6.0/bcel-6.0.pom (19 kB at 934 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/40/commons-parent-40.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/40/commons-parent-40.pom (64 kB at 3.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.12/junit-4.12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.12/junit-4.12.pom (24 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-i18n/1.0-beta-6/plexus-i18n-1.0-beta-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-i18n/1.0-beta-6/plexus-i18n-1.0-beta-6.pom (771 B at 43 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.4/plexus-components-1.1.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.4/plexus-components-1.1.4.pom (2.1 kB at 109 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.7/plexus-utils-3.0.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.7/plexus-utils-3.0.7.pom (2.5 kB at 140 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/net/sf/clirr/clirr-core/0.6/clirr-core-0.6.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/bcel/bcel/6.0/bcel-6.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.1/commons-lang-2.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2/commons-collections-3.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/net/sf/clirr/clirr-core/0.6/clirr-core-0.6.jar (69 kB at 2.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-i18n/1.0-beta-6/plexus-i18n-1.0-beta-6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/reporting/maven-reporting-api/2.0.6/maven-reporting-api-2.0.6.jar (9.9 kB at 432 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.7/plexus-utils-3.0.7.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-lang/commons-lang/2.1/commons-lang-2.1.jar (208 kB at 7.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-i18n/1.0-beta-6/plexus-i18n-1.0-beta-6.jar (12 kB at 300 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/bcel/bcel/6.0/bcel-6.0.jar (671 kB at 15 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-collections/commons-collections/3.2/commons-collections-3.2.jar (571 kB at 12 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.7/plexus-utils-3.0.7.jar (230 kB at 4.4 MB/s)
[INFO] Skipping execution
[INFO] Skipping execution
[INFO] 
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ google-cloud-video-intelligence-parent ---
[INFO] --- maven-install-plugin:2.4:install (default-install) @ google-cloud-video-intelligence-bom ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/pom.xml to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence-parent/1.5.9/google-cloud-video-intelligence-parent-1.5.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/pom.xml to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence-bom/1.5.9/google-cloud-video-intelligence-bom-1.5.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/target/google-cloud-video-intelligence-parent-1.5.9-tests.jar to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence-parent/1.5.9/google-cloud-video-intelligence-parent-1.5.9-tests.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/target/google-cloud-video-intelligence-bom-1.5.9-tests.jar to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence-bom/1.5.9/google-cloud-video-intelligence-bom-1.5.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p3beta1 >--
[INFO] 
[INFO] 
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1beta2 >--
[INFO] Building proto-google-cloud-video-intelligence-v1p3beta1 0.87.9   [3/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] Building proto-google-cloud-video-intelligence-v1beta2 0.87.9     [4/13]
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p1beta1 >--
[INFO] ----< com.google.api.grpc:proto-google-cloud-video-intelligence-v1 >----
[INFO] Building proto-google-cloud-video-intelligence-v1 1.5.9           [6/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] Building proto-google-cloud-video-intelligence-v1p1beta1 0.87.9   [5/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.pom (8.1 kB at 427 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-resources-plugin/2.6/maven-resources-plugin-2.6.jar (30 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/flatten-maven-plugin/1.2.5/flatten-maven-plugin-1.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/flatten-maven-plugin/1.2.5/flatten-maven-plugin-1.2.5.pom (9.7 kB at 512 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/flatten-maven-plugin/1.2.5/flatten-maven-plugin-1.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/flatten-maven-plugin/1.2.5/flatten-maven-plugin-1.2.5.jar (112 kB at 5.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.8.1/maven-compiler-plugin-3.8.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.8.1/maven-compiler-plugin-3.8.1.pom (12 kB at 656 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.8.1/maven-compiler-plugin-3.8.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-compiler-plugin/3.8.1/maven-compiler-plugin-3.8.1.jar (62 kB at 3.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/3.0.0-M5/maven-surefire-plugin-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/3.0.0-M5/maven-surefire-plugin-3.0.0-M5.pom (8.0 kB at 424 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/3.0.0-M5/surefire-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire/3.0.0-M5/surefire-3.0.0-M5.pom (27 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/3.0.0-M5/maven-surefire-plugin-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/plugins/maven-surefire-plugin/3.0.0-M5/maven-surefire-plugin-3.0.0-M5.jar (43 kB at 2.2 MB/s)
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in proto-google-cloud-video-intelligence-v1p3beta1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom
[WARNING] *****************************************************************
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in proto-google-cloud-video-intelligence-v1beta2:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in proto-google-cloud-video-intelligence-v1p1beta1:
[WARNING] The following plugins are not marked @threadSafe in proto-google-cloud-video-intelligence-v1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom (5.6 kB at 242 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-parent/3.14.0/protobuf-parent-3.14.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-parent/3.14.0/protobuf-parent-3.14.0.pom (7.7 kB at 427 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.pom (2.2 kB at 128 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom (0 B at 0 B/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom (0 B at 0 B/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.pom (0 B at 0 B/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar (1.7 MB at 20 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar (1.6 MB at 15 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.pom (6.7 kB at 336 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar (1.7 MB at 26 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.pom (1.9 kB at 106 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.pom (1.7 kB at 100 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.pom (2.0 kB at 119 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.pom (1.3 kB at 66 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.pom (5.8 kB at 341 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.12/plexus-interpolation-1.12.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java/3.14.0/protobuf-java-3.14.0.jar (1.7 MB at 8.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.12/plexus-interpolation-1.12.pom (889 B at 49 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.pom (2.9 kB at 159 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/10/spice-parent-10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/spice/spice-parent/10/spice-parent-10.pom (3.0 kB at 168 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/3/forge-parent-3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar (1.6 MB at 6.1 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/3/forge-parent-3.pom (5.0 kB at 265 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.pom (890 B at 37 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.15/plexus-components-1.1.15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.1.15/plexus-components-1.1.15.pom (2.8 kB at 158 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.0.6/maven-plugin-parameter-documenter-2.0.6.jar (21 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.0.6/maven-error-diagnostics-2.0.6.jar (14 kB at 681 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/doxia/doxia-sink-api/1.0-alpha-7/doxia-sink-api-1.0-alpha-7.jar (5.9 kB at 283 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.0.6/maven-plugin-descriptor-2.0.6.jar (37 kB at 2.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.0.6/maven-core-2.0.6.jar (152 kB at 6.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.0.6/maven-monitor-2.0.6.jar (10 kB at 301 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/1.1/maven-filtering-1.1.jar (43 kB at 1.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/plexus/plexus-build-api/0.0.4/plexus-build-api-0.0.4.jar (6.8 kB at 179 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.13/plexus-interpolation-1.13.jar (61 kB at 1.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.5/plexus-utils-2.0.5.jar (223 kB at 4.5 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar (1.6 MB at 3.8 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.2.5/maven-model-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/grpc/proto-google-common-protos/2.0.1/proto-google-common-protos-2.0.1.jar (1.6 MB at 3.2 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.2.5/maven-model-3.2.5.pom (4.2 kB at 224 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.2.5/maven-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/3.2.5/maven-3.2.5.pom (22 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.20/plexus-utils-3.0.20.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/3.0.20/plexus-utils-3.0.20.pom (3.8 kB at 238 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.2.5/maven-model-builder-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.2.5/maven-model-builder-3.2.5.pom (3.0 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.21/plexus-interpolation-1.21.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.21/plexus-interpolation-1.21.pom (1.5 kB at 81 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.3.1/plexus-components-1.3.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/1.3.1/plexus-components-1.3.1.pom (3.1 kB at 180 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.2.5/maven-artifact-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.2.5/maven-artifact-3.2.5.pom (2.3 kB at 138 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.2.5/maven-core-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.2.5/maven-core-3.2.5.pom (8.1 kB at 474 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.2.5/maven-settings-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.2.5/maven-settings-3.2.5.pom (2.2 kB at 114 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.2.5/maven-settings-builder-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.2.5/maven-settings-builder-3.2.5.pom (2.6 kB at 144 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.2.5/maven-repository-metadata-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.2.5/maven-repository-metadata-3.2.5.pom (2.2 kB at 106 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.2.5/maven-aether-provider-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.2.5/maven-aether-provider-3.2.5.pom (4.2 kB at 224 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-api/1.0.0.v20140518/aether-api-1.0.0.v20140518.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-api/1.0.0.v20140518/aether-api-1.0.0.v20140518.pom (1.9 kB at 105 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether/1.0.0.v20140518/aether-1.0.0.v20140518.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether/1.0.0.v20140518/aether-1.0.0.v20140518.pom (30 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-spi/1.0.0.v20140518/aether-spi-1.0.0.v20140518.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-spi/1.0.0.v20140518/aether-spi-1.0.0.v20140518.pom (2.1 kB at 108 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-util/1.0.0.v20140518/aether-util-1.0.0.v20140518.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-util/1.0.0.v20140518/aether-util-1.0.0.v20140518.pom (2.2 kB at 110 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-impl/1.0.0.v20140518/aether-impl-1.0.0.v20140518.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-impl/1.0.0.v20140518/aether-impl-1.0.0.v20140518.pom (3.5 kB at 204 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.plexus/0.3.0.M1/org.eclipse.sisu.plexus-0.3.0.M1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.plexus/0.3.0.M1/org.eclipse.sisu.plexus-0.3.0.M1.pom (4.7 kB at 235 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/sisu-plexus/0.3.0.M1/sisu-plexus-0.3.0.M1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/sisu-plexus/0.3.0.M1/sisu-plexus-0.3.0.M1.pom (13 kB at 697 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/enterprise/cdi-api/1.0/cdi-api-1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/enterprise/cdi-api/1.0/cdi-api-1.0.pom (1.4 kB at 84 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-api-parent/1.0/weld-api-parent-1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-api-parent/1.0/weld-api-parent-1.0.pom (2.4 kB at 147 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-api-bom/1.0/weld-api-bom-1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-api-bom/1.0/weld-api-bom-1.0.pom (7.9 kB at 465 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-parent/6/weld-parent-6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/jboss/weld/weld-parent/6/weld-parent-6.pom (21 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/annotation/jsr250-api/1.0/jsr250-api-1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/annotation/jsr250-api/1.0/jsr250-api-1.0.pom (1.0 kB at 57 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.inject/0.3.0.M1/org.eclipse.sisu.inject-0.3.0.M1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.inject/0.3.0.M1/org.eclipse.sisu.inject-0.3.0.M1.pom (2.6 kB at 150 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/sisu-inject/0.3.0.M1/sisu-inject-0.3.0.M1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/sisu-inject/0.3.0.M1/sisu-inject-0.3.0.M1.pom (14 kB at 841 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.1/plexus-classworlds-2.5.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.1/plexus-classworlds-2.5.1.pom (5.0 kB at 250 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/3.2.3/sisu-guice-3.2.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/3.2.3/sisu-guice-3.2.3.pom (11 kB at 643 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-parent/3.2.3/guice-parent-3.2.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/inject/guice-parent/3.2.3/guice-parent-3.2.3.pom (13 kB at 642 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/38/forge-parent-38.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/forge/forge-parent/38/forge-parent-38.pom (19 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/aopalliance/aopalliance/1.0/aopalliance-1.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/aopalliance/aopalliance/1.0/aopalliance-1.0.pom (363 B at 17 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/16.0.1/guava-16.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/16.0.1/guava-16.0.1.pom (6.1 kB at 339 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/16.0.1/guava-parent-16.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/16.0.1/guava-parent-16.0.1.pom (7.3 kB at 432 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.2/plexus-classworlds-2.5.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.2/plexus-classworlds-2.5.2.pom (7.3 kB at 430 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.2.5/maven-plugin-api-3.2.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.2.5/maven-plugin-api-3.2.5.pom (3.0 kB at 178 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.9.0/maven-artifact-transfer-0.9.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.9.0/maven-artifact-transfer-0.9.0.pom (7.6 kB at 447 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7/plexus-component-annotations-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-component-annotations/1.7/plexus-component-annotations-1.7.pom (748 B at 47 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.7/plexus-containers-1.7.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-containers/1.7/plexus-containers-1.7.pom (4.8 kB at 280 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.0.0/maven-common-artifact-filters-3.0.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.0.0/maven-common-artifact-filters-3.0.0.pom (4.8 kB at 267 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.5/slf4j-api-1.7.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.5/slf4j-api-1.7.5.pom (2.7 kB at 158 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.7.5/slf4j-parent-1.7.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.7.5/slf4j-parent-1.7.5.pom (12 kB at 656 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.2.5/maven-model-3.2.5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.21/plexus-interpolation-1.21.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.2.5/maven-model-builder-3.2.5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.2.5/maven-artifact-3.2.5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.2.5/maven-core-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/3.2.5/maven-artifact-3.2.5.jar (55 kB at 2.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.2.5/maven-settings-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.21/plexus-interpolation-1.21.jar (62 kB at 2.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.2.5/maven-settings-builder-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/3.2.5/maven-model-3.2.5.jar (161 kB at 5.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.2.5/maven-repository-metadata-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model-builder/3.2.5/maven-model-builder-3.2.5.jar (170 kB at 4.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.2.5/maven-aether-provider-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/3.2.5/maven-settings-3.2.5.jar (43 kB at 1.1 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings-builder/3.2.5/maven-settings-builder-3.2.5.jar (44 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-spi/1.0.0.v20140518/aether-spi-1.0.0.v20140518.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-impl/1.0.0.v20140518/aether-impl-1.0.0.v20140518.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/3.2.5/maven-core-3.2.5.jar (608 kB at 13 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-api/1.0.0.v20140518/aether-api-1.0.0.v20140518.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/3.2.5/maven-repository-metadata-3.2.5.jar (26 kB at 564 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.plexus/0.3.0.M1/org.eclipse.sisu.plexus-0.3.0.M1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-aether-provider/3.2.5/maven-aether-provider-3.2.5.jar (66 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/enterprise/cdi-api/1.0/cdi-api-1.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-spi/1.0.0.v20140518/aether-spi-1.0.0.v20140518.jar (31 kB at 530 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/annotation/jsr250-api/1.0/jsr250-api-1.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-api/1.0.0.v20140518/aether-api-1.0.0.v20140518.jar (136 kB at 2.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.inject/0.3.0.M1/org.eclipse.sisu.inject-0.3.0.M1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/aether/aether-impl/1.0.0.v20140518/aether-impl-1.0.0.v20140518.jar (172 kB at 2.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/3.2.3/sisu-guice-3.2.3-no_aop.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.plexus/0.3.0.M1/org.eclipse.sisu.plexus-0.3.0.M1.jar (201 kB at 3.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/aopalliance/aopalliance/1.0/aopalliance-1.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/annotation/jsr250-api/1.0/jsr250-api-1.0.jar (5.8 kB at 80 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/16.0.1/guava-16.0.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/enterprise/cdi-api/1.0/cdi-api-1.0.jar (45 kB at 591 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.2/plexus-classworlds-2.5.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/eclipse/sisu/org.eclipse.sisu.inject/0.3.0.M1/org.eclipse.sisu.inject-0.3.0.M1.jar (340 kB at 3.6 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/aopalliance/aopalliance/1.0/aopalliance-1.0.jar (4.5 kB at 48 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.9.0/maven-artifact-transfer-0.9.0.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.2.5/maven-plugin-api-3.2.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/sonatype/sisu/sisu-guice/3.2.3/sisu-guice-3.2.3-no_aop.jar (398 kB at 4.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.0.0/maven-common-artifact-filters-3.0.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-classworlds/2.5.2/plexus-classworlds-2.5.2.jar (53 kB at 507 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.5/slf4j-api-1.7.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-artifact-transfer/0.9.0/maven-artifact-transfer-0.9.0.jar (123 kB at 1.1 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/3.2.5/maven-plugin-api-3.2.5.jar (46 kB at 394 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.0.0/maven-common-artifact-filters-3.0.0.jar (57 kB at 485 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.7.5/slf4j-api-1.7.5.jar (26 kB at 210 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/16.0.1/guava-16.0.1.jar (2.2 MB at 15 MB/s)
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-incremental/1.1/maven-shared-incremental-1.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-incremental/1.1/maven-shared-incremental-1.1.pom (4.7 kB at 250 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.2.1/maven-plugin-api-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-api/2.2.1/maven-plugin-api-2.2.1.pom (1.5 kB at 56 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.2.1/maven-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven/2.2.1/maven-2.2.1.pom (22 kB at 1.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.2.1/maven-core-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-core/2.2.1/maven-core-2.2.1.pom (12 kB at 612 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.2.1/maven-settings-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-settings/2.2.1/maven-settings-2.2.1.pom (2.2 kB at 128 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.2.1/maven-model-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-model/2.2.1/maven-model-2.2.1.pom (3.2 kB at 191 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.2.1/maven-plugin-parameter-documenter-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-parameter-documenter/2.2.1/maven-plugin-parameter-documenter-2.2.1.pom (2.0 kB at 115 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-jdk14/1.5.6/slf4j-jdk14-1.5.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-jdk14/1.5.6/slf4j-jdk14-1.5.6.pom (1.9 kB at 112 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.5.6/slf4j-parent-1.5.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-parent/1.5.6/slf4j-parent-1.5.6.pom (7.9 kB at 440 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.5.6/slf4j-api-1.5.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/slf4j-api/1.5.6/slf4j-api-1.5.6.pom (3.0 kB at 176 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.5.6/jcl-over-slf4j-1.5.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/slf4j/jcl-over-slf4j/1.5.6/jcl-over-slf4j-1.5.6.pom (2.2 kB at 120 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.2.1/maven-profile-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-profile/2.2.1/maven-profile-2.2.1.pom (2.2 kB at 128 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.2.1/maven-artifact-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact/2.2.1/maven-artifact-2.2.1.pom (1.6 kB at 83 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.2.1/maven-repository-metadata-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-repository-metadata/2.2.1/maven-repository-metadata-2.2.1.pom (1.9 kB at 98 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.2.1/maven-error-diagnostics-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-error-diagnostics/2.2.1/maven-error-diagnostics-2.2.1.pom (1.7 kB at 95 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.2.1/maven-project-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-project/2.2.1/maven-project-2.2.1.pom (2.8 kB at 154 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.2.1/maven-artifact-manager-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-artifact-manager/2.2.1/maven-artifact-manager-2.2.1.pom (3.1 kB at 183 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.2.1/maven-plugin-registry-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-registry/2.2.1/maven-plugin-registry-2.2.1.pom (1.9 kB at 102 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.2.1/maven-plugin-descriptor-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-plugin-descriptor/2.2.1/maven-plugin-descriptor-2.2.1.pom (2.1 kB at 121 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.2.1/maven-monitor-2.2.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-monitor/2.2.1/maven-monitor-2.2.1.pom (1.3 kB at 74 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/0.1/maven-shared-utils-0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-utils/0.1/maven-shared-utils-0.1.pom (4.0 kB at 225 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/18/maven-shared-components-18.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/18/maven-shared-components-18.pom (4.9 kB at 247 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.pom (5.1 kB at 300 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/0.9.10/plexus-languages-0.9.10.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/0.9.10/plexus-languages-0.9.10.pom (4.1 kB at 230 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.pom (2.9 kB at 173 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.8.4/plexus-compiler-api-2.8.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.8.4/plexus-compiler-api-2.8.4.pom (867 B at 51 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.8.4/plexus-compiler-2.8.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler/2.8.4/plexus-compiler-2.8.4.pom (6.0 kB at 335 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/4.0/plexus-components-4.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-components/4.0/plexus-components-4.0.pom (2.7 kB at 156 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.8.4/plexus-compiler-manager-2.8.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.8.4/plexus-compiler-manager-2.8.4.pom (692 B at 41 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.8.4/plexus-compiler-javac-2.8.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.8.4/plexus-compiler-javac-2.8.4.pom (771 B at 45 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.8.4/plexus-compilers-2.8.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compilers/2.8.4/plexus-compilers-2.8.4.pom (1.3 kB at 79 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.4/plexus-utils-2.0.4.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-incremental/1.1/maven-shared-incremental-1.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.8.4/plexus-compiler-api-2.8.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-incremental/1.1/maven-shared-incremental-1.1.jar (14 kB at 752 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.8.4/plexus-compiler-manager-2.8.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/0.9.10/plexus-java-0.9.10.jar (39 kB at 1.9 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-api/2.8.4/plexus-compiler-api-2.8.4.jar (27 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.8.4/plexus-compiler-javac-2.8.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/6.2/asm-6.2.jar (111 kB at 4.8 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/2.0.4/plexus-utils-2.0.4.jar (222 kB at 8.5 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-manager/2.8.4/plexus-compiler-manager-2.8.4.jar (4.7 kB at 138 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-compiler-javac/2.8.4/plexus-compiler-javac-2.8.4.jar (21 kB at 575 kB/s)
[INFO] Changes detected - recompiling the module!
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 46 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/classes
[INFO] Compiling 46 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/classes
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 115 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/classes
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 90 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/classes
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M5/surefire-junit47-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M5/surefire-junit47-3.0.0-M5.pom (8.3 kB at 149 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/3.0.0-M5/surefire-providers-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/3.0.0-M5/surefire-providers-3.0.0-M5.pom (2.5 kB at 110 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M5/common-junit48-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M5/common-junit48-3.0.0-M5.pom (8.0 kB at 382 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M5/common-junit4-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M5/common-junit4-3.0.0-M5.pom (2.9 kB at 164 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M5/common-junit3-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M5/common-junit3-3.0.0-M5.pom (2.6 kB at 145 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M5/surefire-api-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M5/surefire-api-3.0.0-M5.pom (3.2 kB at 179 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M5/surefire-logger-api-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M5/surefire-logger-api-3.0.0-M5.pom (3.7 kB at 115 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-shared-utils/3.0.0-M4/surefire-shared-utils-3.0.0-M4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-shared-utils/3.0.0-M4/surefire-shared-utils-3.0.0-M4.pom (3.9 kB at 217 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M5/common-java5-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M5/common-java5-3.0.0-M5.pom (2.6 kB at 90 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M5/surefire-grouper-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M5/surefire-grouper-3.0.0-M5.pom (3.1 kB at 130 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M5/maven-surefire-common-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M5/maven-surefire-common-3.0.0-M5.pom (9.6 kB at 536 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M5/surefire-extensions-api-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M5/surefire-extensions-api-3.0.0-M5.pom (4.0 kB at 144 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M5/surefire-booter-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M5/surefire-booter-3.0.0-M5.pom (4.8 kB at 101 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-spi/3.0.0-M5/surefire-extensions-spi-3.0.0-M5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-spi/3.0.0-M5/surefire-extensions-spi-3.0.0-M5.pom (1.6 kB at 95 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.5/plexus-java-1.0.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.5/plexus-java-1.0.5.pom (4.6 kB at 243 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/1.0.5/plexus-languages-1.0.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-languages/1.0.5/plexus-languages-1.0.5.pom (3.9 kB at 163 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/6.2/plexus-6.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/6.2/plexus-6.2.pom (24 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.2/asm-7.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.2/asm-7.2.pom (2.9 kB at 164 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M5/common-junit48-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M5/surefire-junit47-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit48/3.0.0-M5/common-junit48-3.0.0-M5.jar (22 kB at 743 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M5/common-junit3-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M5/common-junit4-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M5/surefire-grouper-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M5/common-java5-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit3/3.0.0-M5/common-junit3-3.0.0-M5.jar (12 kB at 326 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M5/surefire-api-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-junit4/3.0.0-M5/common-junit4-3.0.0-M5.jar (25 kB at 508 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-grouper/3.0.0-M5/surefire-grouper-3.0.0-M5.jar (40 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M5/surefire-logger-api-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M5/maven-surefire-common-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-api/3.0.0-M5/surefire-api-3.0.0-M5.jar (144 kB at 3.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M5/surefire-extensions-api-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit47/3.0.0-M5/surefire-junit47-3.0.0-M5.jar (91 kB at 1.0 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/common-java5/3.0.0-M5/common-java5-3.0.0-M5.jar (16 kB at 291 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M5/surefire-booter-3.0.0-M5.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-spi/3.0.0-M5/surefire-extensions-spi-3.0.0-M5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-logger-api/3.0.0-M5/surefire-logger-api-3.0.0-M5.jar (14 kB at 235 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/maven-surefire-common/3.0.0-M5/maven-surefire-common-3.0.0-M5.jar (311 kB at 3.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.5/plexus-java-1.0.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-booter/3.0.0-M5/surefire-booter-3.0.0-M5.jar (106 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.2/asm-7.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-spi/3.0.0-M5/surefire-extensions-spi-3.0.0-M5.jar (7.9 kB at 105 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-extensions-api/3.0.0-M5/surefire-extensions-api-3.0.0-M5.jar (24 kB at 375 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-shared-utils/3.0.0-M4/surefire-shared-utils-3.0.0-M4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-java/1.0.5/plexus-java-1.0.5.jar (52 kB at 501 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/ow2/asm/asm/7.2/asm-7.2.jar (115 kB at 999 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-shared-utils/3.0.0-M4/surefire-shared-utils-3.0.0-M4.jar (1.9 MB at 10 MB/s)
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/proto-google-cloud-video-intelligence-v1beta2-0.87.9.jar
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/proto-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ proto-google-cloud-video-intelligence-v1p1beta1 >>>
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ proto-google-cloud-video-intelligence-v1beta2 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 46 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/classes
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 46 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/classes
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/FaceAnnotation.java:[34,5] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[140,82] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[145,60] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[963,63] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5371,65] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5377,74] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5384,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5385,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5386,50] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5769,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5770,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5771,50] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5776,54] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5777,54] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5778,54] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/proto-google-cloud-video-intelligence-v1-1.5.9.jar
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ proto-google-cloud-video-intelligence-v1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/proto-google-cloud-video-intelligence-v1-1.5.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ proto-google-cloud-video-intelligence-v1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/resources
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 90 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/classes
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ proto-google-cloud-video-intelligence-v1p3beta1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 115 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/classes
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ proto-google-cloud-video-intelligence-v1beta2 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/proto-google-cloud-video-intelligence-v1beta2-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1beta2/0.87.9/proto-google-cloud-video-intelligence-v1beta2-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1beta2/0.87.9/proto-google-cloud-video-intelligence-v1beta2-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/proto-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1beta2/0.87.9/proto-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p2beta1 >--
[INFO] Building proto-google-cloud-video-intelligence-v1p2beta1 0.87.9   [7/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in proto-google-cloud-video-intelligence-v1p2beta1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 54 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/classes
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ proto-google-cloud-video-intelligence-v1p1beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p1beta1/0.87.9/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p1beta1/0.87.9/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p1beta1/0.87.9/proto-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1beta2 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1beta2 0.87.9      [8/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in grpc-google-cloud-video-intelligence-v1beta2:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-api/1.34.1/grpc-api-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-api/1.34.1/grpc-api-1.34.1.pom (2.6 kB at 64 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-context/1.34.1/grpc-context-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-context/1.34.1/grpc-context-1.34.1.pom (1.2 kB at 52 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/3.0.2/jsr305-3.0.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/3.0.2/jsr305-3.0.2.pom (4.3 kB at 214 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/30.1-android/guava-30.1-android.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/30.1-android/guava-30.1-android.pom (12 kB at 611 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/30.1-android/guava-parent-30.1-android.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/30.1-android/guava-parent-30.1-android.pom (13 kB at 701 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/failureaccess/1.0.1/failureaccess-1.0.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/failureaccess/1.0.1/failureaccess-1.0.1.pom (2.4 kB at 80 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/26.0-android/guava-parent-26.0-android.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava-parent/26.0-android/guava-parent-26.0-android.pom (10 kB at 364 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/listenablefuture/9999.0-empty-to-avoid-conflict-with-guava/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/listenablefuture/9999.0-empty-to-avoid-conflict-with-guava/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.pom (2.3 kB at 108 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/checkerframework/checker-compat-qual/2.5.5/checker-compat-qual-2.5.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/checkerframework/checker-compat-qual/2.5.5/checker-compat-qual-2.5.5.pom (2.7 kB at 95 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/j2objc/j2objc-annotations/1.3/j2objc-annotations-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/j2objc/j2objc-annotations/1.3/j2objc-annotations-1.3.pom (2.8 kB at 132 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_annotations/2.5.0/error_prone_annotations-2.5.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_annotations/2.5.0/error_prone_annotations-2.5.0.pom (2.1 kB at 111 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_parent/2.5.0/error_prone_parent-2.5.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_parent/2.5.0/error_prone_parent-2.5.0.pom (7.0 kB at 349 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-annotations/1.19/animal-sniffer-annotations-1.19.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-annotations/1.19/animal-sniffer-annotations-1.19.pom (2.6 kB at 129 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-parent/1.19/animal-sniffer-parent-1.19.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-parent/1.19/animal-sniffer-parent-1.19.pom (9.4 kB at 495 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-stub/1.34.1/grpc-stub-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-stub/1.34.1/grpc-stub-1.34.1.pom (2.6 kB at 126 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf/1.34.1/grpc-protobuf-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf/1.34.1/grpc-protobuf-1.34.1.pom (3.7 kB at 195 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf-lite/1.34.1/grpc-protobuf-lite-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf-lite/1.34.1/grpc-protobuf-lite-1.34.1.pom (2.9 kB at 150 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-api/1.34.1/grpc-api-1.34.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-context/1.34.1/grpc-context-1.34.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/3.0.2/jsr305-3.0.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_annotations/2.5.0/error_prone_annotations-2.5.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-context/1.34.1/grpc-context-1.34.1.jar (31 kB at 874 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-stub/1.34.1/grpc-stub-1.34.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-annotations/1.19/animal-sniffer-annotations-1.19.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-api/1.34.1/grpc-api-1.34.1.jar (254 kB at 4.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/findbugs/jsr305/3.0.2/jsr305-3.0.2.jar (20 kB at 376 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-stub/1.34.1/grpc-stub-1.34.1.jar (50 kB at 2.5 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/errorprone/error_prone_annotations/2.5.0/error_prone_annotations-2.5.0.jar (14 kB at 374 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf/1.34.1/grpc-protobuf-1.34.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/30.1-android/guava-30.1-android.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/mojo/animal-sniffer-annotations/1.19/animal-sniffer-annotations-1.19.jar (3.5 kB at 87 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf-lite/1.34.1/grpc-protobuf-lite-1.34.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/failureaccess/1.0.1/failureaccess-1.0.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/guava/listenablefuture/9999.0-empty-to-avoid-conflict-with-guava/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf/1.34.1/grpc-protobuf-1.34.1.jar (5.2 kB at 77 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/checkerframework/checker-compat-qual/2.5.5/checker-compat-qual-2.5.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/failureaccess/1.0.1/failureaccess-1.0.1.jar (4.6 kB at 67 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/j2objc/j2objc-annotations/1.3/j2objc-annotations-1.3.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-protobuf-lite/1.34.1/grpc-protobuf-lite-1.34.1.jar (7.6 kB at 105 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/listenablefuture/9999.0-empty-to-avoid-conflict-with-guava/listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar (2.2 kB at 26 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/j2objc/j2objc-annotations/1.3/j2objc-annotations-1.3.jar (8.8 kB at 102 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/checkerframework/checker-compat-qual/2.5.5/checker-compat-qual-2.5.5.jar (5.9 kB at 69 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/guava/guava/30.1-android/guava-30.1-android.jar (2.7 MB at 10 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/classes
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/grpc-google-cloud-video-intelligence-v1beta2-0.87.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/grpc-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar
[INFO] 
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ grpc-google-cloud-video-intelligence-v1beta2 >>>
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ proto-google-cloud-video-intelligence-v1p2beta1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 54 source files to /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/classes
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/classes
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/FaceAnnotation.java:[34,5] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[140,82] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[145,60] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[963,63] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5371,65] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5377,74] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5384,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5385,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5386,50] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5769,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5770,50] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5771,50] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5776,54] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5777,54] com.google.cloud.videointelligence.v1.FaceAnnotation in com.google.cloud.videointelligence.v1 has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/java/com/google/cloud/videointelligence/v1/VideoAnnotationResults.java:[5778,54] com.google.cloud.videointelligence.v1.FaceAnnotationOrBuilder in com.google.cloud.videointelligence.v1 has been deprecated
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ proto-google-cloud-video-intelligence-v1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/proto-google-cloud-video-intelligence-v1-1.5.9.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1/1.5.9/proto-google-cloud-video-intelligence-v1-1.5.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1/1.5.9/proto-google-cloud-video-intelligence-v1-1.5.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/proto-google-cloud-video-intelligence-v1-1.5.9-tests.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1/1.5.9/proto-google-cloud-video-intelligence-v1-1.5.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p1beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p1beta1 0.87.9    [9/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in grpc-google-cloud-video-intelligence-v1p1beta1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ grpc-google-cloud-video-intelligence-v1beta2 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/grpc-google-cloud-video-intelligence-v1beta2-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1beta2/0.87.9/grpc-google-cloud-video-intelligence-v1beta2-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1beta2/0.87.9/grpc-google-cloud-video-intelligence-v1beta2-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/grpc-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1beta2/0.87.9/grpc-google-cloud-video-intelligence-v1beta2-0.87.9-tests.jar
[INFO] 
[INFO] ----< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1 >-----
[INFO] Building grpc-google-cloud-video-intelligence-v1 1.5.9           [10/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in grpc-google-cloud-video-intelligence-v1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/classes
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/classes
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ grpc-google-cloud-video-intelligence-v1p1beta1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/grpc-google-cloud-video-intelligence-v1-1.5.9.jar
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/classes
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ grpc-google-cloud-video-intelligence-v1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/grpc-google-cloud-video-intelligence-v1-1.5.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ grpc-google-cloud-video-intelligence-v1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ grpc-google-cloud-video-intelligence-v1p1beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p1beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p1beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p1beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p1beta1-0.87.9-tests.jar
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/classes
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ grpc-google-cloud-video-intelligence-v1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/grpc-google-cloud-video-intelligence-v1-1.5.9.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1/1.5.9/grpc-google-cloud-video-intelligence-v1-1.5.9.jar
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ proto-google-cloud-video-intelligence-v1p3beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1/1.5.9/grpc-google-cloud-video-intelligence-v1-1.5.9.pom
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/grpc-google-cloud-video-intelligence-v1-1.5.9-tests.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1/1.5.9/grpc-google-cloud-video-intelligence-v1-1.5.9-tests.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p3beta1/0.87.9/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p3beta1/0.87.9/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p3beta1/0.87.9/proto-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p3beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p3beta1 0.87.9   [11/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in grpc-google-cloud-video-intelligence-v1p3beta1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/classes
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ proto-google-cloud-video-intelligence-v1p2beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ grpc-google-cloud-video-intelligence-v1p3beta1 >>>
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p2beta1/0.87.9/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p2beta1/0.87.9/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/proto-google-cloud-video-intelligence-v1p2beta1/0.87.9/proto-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p2beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p2beta1 0.87.9   [12/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in grpc-google-cloud-video-intelligence-v1p2beta1:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/classes
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/classes
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ grpc-google-cloud-video-intelligence-v1p3beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p3beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p3beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p3beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p3beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[WARNING] JAR will be empty - no content was marked for inclusion!
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ grpc-google-cloud-video-intelligence-v1p2beta1 >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/classes
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ grpc-google-cloud-video-intelligence-v1p2beta1 <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p2beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/.flattened-pom.xml to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p2beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar to /root/.m2/repository/com/google/api/grpc/grpc-google-cloud-video-intelligence-v1p2beta1/0.87.9/grpc-google-cloud-video-intelligence-v1p2beta1-0.87.9-tests.jar
[INFO] 
[INFO] ----------< com.google.cloud:google-cloud-video-intelligence >----------
[INFO] Building Google Cloud Video Intelligence 1.5.9                   [13/13]
[INFO] --------------------------------[ jar ]---------------------------------
[WARNING] *****************************************************************
[WARNING] * Your build is requesting parallel execution, but project      *
[WARNING] * contains the following plugin(s) that have goals not marked   *
[WARNING] * as @threadSafe to support parallel building.                  *
[WARNING] * While this /may/ work fine, please look for plugin updates    *
[WARNING] * and/or request plugins be made thread-safe.                   *
[WARNING] * If reporting an issue, report it against the plugin in        *
[WARNING] * question, not against maven-core                              *
[WARNING] *****************************************************************
[WARNING] The following plugins are not marked @threadSafe in Google Cloud Video Intelligence:
[WARNING] org.codehaus.mojo:clirr-maven-plugin:2.8
[WARNING] Enable debug to see more precisely which goals are not marked @threadSafe.
[WARNING] *****************************************************************
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/api-common/1.10.1/api-common-1.10.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/api-common/1.10.1/api-common-1.10.1.pom (2.0 kB at 91 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.pom (14 kB at 762 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/net/java/jvnet-parent/3/jvnet-parent-3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/net/java/jvnet-parent/3/jvnet-parent-3.pom (4.8 kB at 266 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-annotations/1.7.4/auto-value-annotations-1.7.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-annotations/1.7.4/auto-value-annotations-1.7.4.pom (2.7 kB at 150 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-parent/1.7.4/auto-value-parent-1.7.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-parent/1.7.4/auto-value-parent-1.7.4.pom (6.1 kB at 339 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax/1.60.1/gax-1.60.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax/1.60.1/gax-1.60.1.pom (2.3 kB at 116 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/threeten/threetenbp/1.5.0/threetenbp-1.5.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/threeten/threetenbp/1.5.0/threetenbp-1.5.0.pom (32 kB at 1.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-oauth2-http/0.22.2/google-auth-library-oauth2-http-0.22.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-oauth2-http/0.22.2/google-auth-library-oauth2-http-0.22.2.pom (3.2 kB at 159 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-parent/0.22.2/google-auth-library-parent-0.22.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-parent/0.22.2/google-auth-library-parent-0.22.2.pom (18 kB at 935 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-credentials/0.22.2/google-auth-library-credentials-0.22.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-credentials/0.22.2/google-auth-library-credentials-0.22.2.pom (2.0 kB at 98 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client/1.38.0/google-http-client-1.38.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client/1.38.0/google-http-client-1.38.0.pom (5.9 kB at 328 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-parent/1.38.0/google-http-client-parent-1.38.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-parent/1.38.0/google-http-client-parent-1.38.0.pom (25 kB at 1.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.5.13/httpclient-4.5.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.5.13/httpclient-4.5.13.pom (6.6 kB at 348 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-client/4.5.13/httpcomponents-client-4.5.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-client/4.5.13/httpcomponents-client-4.5.13.pom (16 kB at 862 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-parent/11/httpcomponents-parent-11.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-parent/11/httpcomponents-parent-11.pom (35 kB at 1.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.4.13/httpcore-4.4.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.4.13/httpcore-4.4.13.pom (5.0 kB at 276 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-core/4.4.13/httpcomponents-core-4.4.13.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcomponents-core/4.4.13/httpcomponents-core-4.4.13.pom (13 kB at 658 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging/1.2/commons-logging-1.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging/1.2/commons-logging-1.2.pom (19 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/34/commons-parent-34.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/34/commons-parent-34.pom (56 kB at 2.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.15/commons-codec-1.15.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.15/commons-codec-1.15.pom (15 kB at 813 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/52/commons-parent-52.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/52/commons-parent-52.pom (79 kB at 4.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-api/0.24.0/opencensus-api-0.24.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-api/0.24.0/opencensus-api-0.24.0.pom (2.2 kB at 124 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-contrib-http-util/0.24.0/opencensus-contrib-http-util-0.24.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-contrib-http-util/0.24.0/opencensus-contrib-http-util-0.24.0.pom (2.4 kB at 122 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-jackson2/1.38.0/google-http-client-jackson2-1.38.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-jackson2/1.38.0/google-http-client-jackson2-1.38.0.pom (3.1 kB at 174 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.12.1/jackson-core-2.12.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.12.1/jackson-core-2.12.1.pom (5.5 kB at 291 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-base/2.12.1/jackson-base-2.12.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/jackson-base/2.12.1/jackson-base-2.12.1.pom (9.3 kB at 546 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1.pom (3.6 kB at 211 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-auth/1.34.1/grpc-auth-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-auth/1.34.1/grpc-auth-1.34.1.pom (2.8 kB at 158 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-netty-shaded/1.34.1/grpc-netty-shaded-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-netty-shaded/1.34.1/grpc-netty-shaded-1.34.1.pom (1.4 kB at 79 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-core/1.34.1/grpc-core-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-core/1.34.1/grpc-core-1.34.1.pom (3.4 kB at 198 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson/2.8.6/gson-2.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson/2.8.6/gson-2.8.6.pom (2.5 kB at 140 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson-parent/2.8.6/gson-parent-2.8.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson-parent/2.8.6/gson-parent-2.8.6.pom (4.4 kB at 201 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/android/annotations/4.1.1.4/annotations-4.1.1.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/android/annotations/4.1.1.4/annotations-4.1.1.4.pom (1.8 kB at 102 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/perfmark/perfmark-api/0.19.0/perfmark-api-0.19.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/perfmark/perfmark-api/0.19.0/perfmark-api-0.19.0.pom (1.5 kB at 91 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-alts/1.34.1/grpc-alts-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-alts/1.34.1/grpc-alts-1.34.1.pom (3.2 kB at 154 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-grpclb/1.34.1/grpc-grpclb-1.34.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-grpclb/1.34.1/grpc-grpclb-1.34.1.pom (3.7 kB at 218 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java-util/3.14.0/protobuf-java-util-3.14.0.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java-util/3.14.0/protobuf-java-util-3.14.0.pom (4.8 kB at 281 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.5/commons-lang3-3.5.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.5/commons-lang3-3.5.pom (23 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/41/commons-parent-41.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/41/commons-parent-41.pom (65 kB at 3.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/conscrypt/conscrypt-openjdk-uber/2.5.1/conscrypt-openjdk-uber-2.5.1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/conscrypt/conscrypt-openjdk-uber/2.5.1/conscrypt-openjdk-uber-2.5.1.pom (1.3 kB at 70 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.13.2/junit-4.13.2.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.13.2/junit-4.13.2.pom (27 kB at 1.4 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/api-common/1.10.1/api-common-1.10.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-oauth2-http/0.22.2/google-auth-library-oauth2-http-0.22.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax/1.60.1/gax-1.60.1.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-annotations/1.7.4/auto-value-annotations-1.7.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/api-common/1.10.1/api-common-1.10.1.jar (49 kB at 2.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client/1.38.0/google-http-client-1.38.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/javax/annotation/javax.annotation-api/1.3.2/javax.annotation-api-1.3.2.jar (27 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.5.13/httpclient-4.5.13.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-oauth2-http/0.22.2/google-auth-library-oauth2-http-0.22.2.jar (115 kB at 4.3 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auto/value/auto-value-annotations/1.7.4/auto-value-annotations-1.7.4.jar (6.6 kB at 227 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging/1.2/commons-logging-1.2.jar
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.15/commons-codec-1.15.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client/1.38.0/google-http-client-1.38.0.jar (288 kB at 5.3 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.4.13/httpcore-4.4.13.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax/1.60.1/gax-1.60.1.jar (335 kB at 5.9 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-contrib-http-util/0.24.0/opencensus-contrib-http-util-0.24.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-logging/commons-logging/1.2/commons-logging-1.2.jar (62 kB at 883 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-jackson2/1.38.0/google-http-client-jackson2-1.38.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-contrib-http-util/0.24.0/opencensus-contrib-http-util-0.24.0.jar (23 kB at 296 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.12.1/jackson-core-2.12.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpclient/4.5.13/httpclient-4.5.13.jar (780 kB at 9.8 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-api/0.24.0/opencensus-api-0.24.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/http-client/google-http-client-jackson2/1.38.0/google-http-client-jackson2-1.38.0.jar (8.5 kB at 95 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/httpcomponents/httpcore/4.4.13/httpcore-4.4.13.jar (329 kB at 3.5 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-auth/1.34.1/grpc-auth-1.34.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.15/commons-codec-1.15.jar (354 kB at 3.7 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-credentials/0.22.2/google-auth-library-credentials-0.22.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1.jar (117 kB at 1.1 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-netty-shaded/1.34.1/grpc-netty-shaded-1.34.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/fasterxml/jackson/core/jackson-core/2.12.1/jackson-core-2.12.1.jar (365 kB at 3.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-core/1.34.1/grpc-core-1.34.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/auth/google-auth-library-credentials/0.22.2/google-auth-library-credentials-0.22.2.jar (5.7 kB at 50 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson/2.8.6/gson-2.8.6.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-auth/1.34.1/grpc-auth-1.34.1.jar (14 kB at 126 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/android/annotations/4.1.1.4/annotations-4.1.1.4.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/opencensus/opencensus-api/0.24.0/opencensus-api-0.24.0.jar (352 kB at 3.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/perfmark/perfmark-api/0.19.0/perfmark-api-0.19.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/android/annotations/4.1.1.4/annotations-4.1.1.4.jar (3.1 kB at 23 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-alts/1.34.1/grpc-alts-1.34.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/perfmark/perfmark-api/0.19.0/perfmark-api-0.19.0.jar (4.7 kB at 33 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-grpclb/1.34.1/grpc-grpclb-1.34.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/code/gson/gson/2.8.6/gson-2.8.6.jar (240 kB at 1.6 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java-util/3.14.0/protobuf-java-util-3.14.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-core/1.34.1/grpc-core-1.34.1.jar (646 kB at 4.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.5/commons-lang3-3.5.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-alts/1.34.1/grpc-alts-1.34.1.jar (313 kB at 1.9 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/conscrypt/conscrypt-openjdk-uber/2.5.1/conscrypt-openjdk-uber-2.5.1.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-grpclb/1.34.1/grpc-grpclb-1.34.1.jar (179 kB at 1.0 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/threeten/threetenbp/1.5.0/threetenbp-1.5.0.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/protobuf/protobuf-java-util/3.14.0/protobuf-java-util-3.14.0.jar (75 kB at 429 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/junit/junit/4.13.2/junit-4.13.2.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.5/commons-lang3-3.5.jar (480 kB at 2.2 MB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1-testlib.jar
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/junit/junit/4.13.2/junit-4.13.2.jar (385 kB at 1.8 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/threeten/threetenbp/1.5.0/threetenbp-1.5.0.jar (516 kB at 2.2 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/google/api/gax-grpc/1.60.1/gax-grpc-1.60.1-testlib.jar (28 kB at 120 kB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/io/grpc/grpc-netty-shaded/1.34.1/grpc-netty-shaded-1.34.1.jar (7.9 MB at 23 MB/s)
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/conscrypt/conscrypt-openjdk-uber/2.5.1/conscrypt-openjdk-uber-2.5.1.jar (4.5 MB at 12 MB/s)
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ google-cloud-video-intelligence ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ google-cloud-video-intelligence ---
[INFO] Generating flattened POM of project com.google.cloud:google-cloud-video-intelligence:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ google-cloud-video-intelligence ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 41 source files to /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/classes
[INFO] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/java/com/google/cloud/videointelligence/v1p3beta1/VideoIntelligenceServiceSettings.java: Some input files use unchecked or unsafe operations.
[INFO] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/java/com/google/cloud/videointelligence/v1p3beta1/VideoIntelligenceServiceSettings.java: Recompile with -Xlint:unchecked for details.
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ google-cloud-video-intelligence ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ google-cloud-video-intelligence ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 23 source files to /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/test-classes
[WARNING] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/java/com/google/cloud/videointelligence/v1p3beta1/StreamingVideoIntelligenceServiceClientTest.java:[99,17] bidiStreamingCall(com.google.api.gax.rpc.ApiStreamObserver<ResponseT>) in com.google.api.gax.rpc.BidiStreamingCallable has been deprecated
[WARNING] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/java/com/google/cloud/videointelligence/v1p3beta1/StreamingVideoIntelligenceServiceClientTest.java:[121,17] bidiStreamingCall(com.google.api.gax.rpc.ApiStreamObserver<ResponseT>) in com.google.api.gax.rpc.BidiStreamingCallable has been deprecated
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ google-cloud-video-intelligence ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:jar (default-jar) @ google-cloud-video-intelligence ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/google-cloud-video-intelligence-1.5.9.jar
[INFO] 
[INFO] --- maven-jar-plugin:3.2.0:test-jar (default) @ google-cloud-video-intelligence ---
[INFO] Building jar: /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/google-cloud-video-intelligence-1.5.9-tests.jar
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:integration-test (default) @ google-cloud-video-intelligence ---
[INFO] Tests are skipped.
[INFO] 
[INFO] --- maven-failsafe-plugin:3.0.0-M4:verify (default) @ google-cloud-video-intelligence ---
[INFO] Tests are skipped.
[INFO] 
[INFO] >>> clirr-maven-plugin:2.8:check (default) > compile @ google-cloud-video-intelligence >>>
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ google-cloud-video-intelligence ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/proto
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ google-cloud-video-intelligence ---
[INFO] Generating flattened POM of project com.google.cloud:google-cloud-video-intelligence:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ google-cloud-video-intelligence ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 41 source files to /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/classes
[INFO] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/java/com/google/cloud/videointelligence/v1p3beta1/VideoIntelligenceServiceSettings.java: Some input files use unchecked or unsafe operations.
[INFO] /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/java/com/google/cloud/videointelligence/v1p3beta1/VideoIntelligenceServiceSettings.java: Recompile with -Xlint:unchecked for details.
[INFO] 
[INFO] <<< clirr-maven-plugin:2.8:check (default) < compile @ google-cloud-video-intelligence <<<
[INFO] 
[INFO] 
[INFO] --- clirr-maven-plugin:2.8:check (default) @ google-cloud-video-intelligence ---
[INFO] Skipping execution
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ google-cloud-video-intelligence ---
[INFO] Installing /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/google-cloud-video-intelligence-1.5.9.jar to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence/1.5.9/google-cloud-video-intelligence-1.5.9.jar
[INFO] Installing /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/.flattened-pom.xml to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence/1.5.9/google-cloud-video-intelligence-1.5.9.pom
[INFO] Installing /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/google-cloud-video-intelligence-1.5.9-tests.jar to /root/.m2/repository/com/google/cloud/google-cloud-video-intelligence/1.5.9/google-cloud-video-intelligence-1.5.9-tests.jar
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO] 
[INFO] Google Cloud Video Intelligence Parent 1.5.9 ....... SUCCESS [  6.550 s]
[INFO] proto-google-cloud-video-intelligence-v1p3beta1 0.87.9 SUCCESS [ 19.005 s]
[INFO] proto-google-cloud-video-intelligence-v1beta2 0.87.9 SUCCESS [ 15.114 s]
[INFO] proto-google-cloud-video-intelligence-v1p1beta1 0.87.9 SUCCESS [ 15.485 s]
[INFO] proto-google-cloud-video-intelligence-v1 1.5.9 ..... SUCCESS [ 17.907 s]
[INFO] proto-google-cloud-video-intelligence-v1p2beta1 0.87.9 SUCCESS [  4.430 s]
[INFO] grpc-google-cloud-video-intelligence-v1p1beta1 0.87.9 SUCCESS [  0.695 s]
[INFO] grpc-google-cloud-video-intelligence-v1beta2 0.87.9  SUCCESS [  2.501 s]
[INFO] grpc-google-cloud-video-intelligence-v1 1.5.9 ...... SUCCESS [  0.959 s]
[INFO] grpc-google-cloud-video-intelligence-v1p2beta1 0.87.9 SUCCESS [  0.514 s]
[INFO] grpc-google-cloud-video-intelligence-v1p3beta1 0.87.9 SUCCESS [  0.768 s]
[INFO] Google Cloud Video Intelligence 1.5.9 .............. SUCCESS [  3.059 s]
[INFO] Google Cloud video-intelligence BOM 1.5.9 .......... SUCCESS [  6.550 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  37.517 s (Wall Clock)
[INFO] Finished at: 2021-02-19T10:32:56Z
[INFO] ------------------------------------------------------------------------
[INFO] Scanning for projects...
[WARNING] 
[WARNING] Some problems were encountered while building the effective model for com.google.cloud:google-cloud-video-intelligence-bom:pom:1.5.9
[WARNING] 'build.plugins.plugin.version' for org.apache.maven.plugins:maven-checkstyle-plugin is missing. @ line 124, column 15
[WARNING] 
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING] 
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[WARNING] 
[INFO] Inspecting build with total of 13 modules...
[INFO] Installing Nexus Staging features:
[INFO]   ... total of 13 executions of maven-deploy-plugin replaced with nexus-staging-maven-plugin
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] Google Cloud Video Intelligence Parent                             [pom]
[INFO] proto-google-cloud-video-intelligence-v1p3beta1                    [jar]
[INFO] proto-google-cloud-video-intelligence-v1beta2                      [jar]
[INFO] proto-google-cloud-video-intelligence-v1p1beta1                    [jar]
[INFO] proto-google-cloud-video-intelligence-v1                           [jar]
[INFO] proto-google-cloud-video-intelligence-v1p2beta1                    [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p1beta1                     [jar]
[INFO] grpc-google-cloud-video-intelligence-v1beta2                       [jar]
[INFO] grpc-google-cloud-video-intelligence-v1                            [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p2beta1                     [jar]
[INFO] grpc-google-cloud-video-intelligence-v1p3beta1                     [jar]
[INFO] Google Cloud Video Intelligence                                    [jar]
[INFO] Google Cloud video-intelligence BOM                                [pom]
[INFO] 
[INFO] ------< com.google.cloud:google-cloud-video-intelligence-parent >-------
[INFO] Building Google Cloud Video Intelligence Parent 1.5.9             [1/13]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-parent ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-parent ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-parent ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence-parent ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence-parent ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p3beta1 >--
[INFO] Building proto-google-cloud-video-intelligence-v1p3beta1 0.87.9   [2/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p3beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1beta2 >--
[INFO] Building proto-google-cloud-video-intelligence-v1beta2 0.87.9     [3/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1beta2/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p1beta1 >--
[INFO] Building proto-google-cloud-video-intelligence-v1p1beta1 0.87.9   [4/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p1beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] ----< com.google.api.grpc:proto-google-cloud-video-intelligence-v1 >----
[INFO] Building proto-google-cloud-video-intelligence-v1 1.5.9           [5/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:proto-google-cloud-video-intelligence-v1p2beta1 >--
[INFO] Building proto-google-cloud-video-intelligence-v1p2beta1 0.87.9   [6/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] Copying 1 resource
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:proto-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/proto-google-cloud-video-intelligence-v1p2beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ proto-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p1beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p1beta1 0.87.9    [7/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p1beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p1beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p1beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1beta2 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1beta2 0.87.9      [8/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1beta2:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1beta2/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1beta2 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] ----< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1 >-----
[INFO] Building grpc-google-cloud-video-intelligence-v1 1.5.9            [9/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p2beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p2beta1 0.87.9   [10/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p2beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p2beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p2beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] --< com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p3beta1 >--
[INFO] Building grpc-google-cloud-video-intelligence-v1p3beta1 0.87.9   [11/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Generating flattened POM of project com.google.api.grpc:grpc-google-cloud-video-intelligence-v1p3beta1:jar:0.87.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/grpc-google-cloud-video-intelligence-v1p3beta1/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No sources to compile
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ grpc-google-cloud-video-intelligence-v1p3beta1 ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] 
[INFO] ----------< com.google.cloud:google-cloud-video-intelligence >----------
[INFO] Building Google Cloud Video Intelligence 1.5.9                   [12/13]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ google-cloud-video-intelligence ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/main/proto
[INFO] 
[INFO] --- flatten-maven-plugin:1.2.5:flatten (flatten) @ google-cloud-video-intelligence ---
[INFO] Generating flattened POM of project com.google.cloud:google-cloud-video-intelligence:jar:1.5.9...
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:compile (default-compile) @ google-cloud-video-intelligence ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence ---
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ google-cloud-video-intelligence ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/resources
[INFO] skip non existing resourceDirectory /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/src/test/proto
[INFO] 
[INFO] --- maven-compiler-plugin:3.8.1:testCompile (default-testCompile) @ google-cloud-video-intelligence ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0-M5:test (default-test) @ google-cloud-video-intelligence ---
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/com/github/stephenc/jcip/jcip-annotations/1.0-1/jcip-annotations-1.0-1.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/com/github/stephenc/jcip/jcip-annotations/1.0-1/jcip-annotations-1.0-1.pom (5.4 kB at 13 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-library/1.3/hamcrest-library-1.3.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/hamcrest/hamcrest-library/1.3/hamcrest-library-1.3.pom (820 B at 34 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/easytesting/fest-assert/1.4/fest-assert-1.4.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/easytesting/fest-assert/1.4/fest-assert-1.4.pom (2.4 kB at 88 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/easytesting/fest/1.0.8/fest-1.0.8.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/easytesting/fest/1.0.8/fest-1.0.8.pom (12 kB at 448 kB/s)
[INFO] Downloading from central: https://repo.maven.apache.org/maven2/org/easytesting/fest-util/1.1.6/fest-util-1.1.6.pom
[INFO] Downloaded from central: https://repo.maven.apache.org/maven2/org/easytesting/fest-util/1.1.6/fest-util-1.1.6.pom (1.6 kB at 56 kB/s)
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClientTest
Feb 19, 2021 10:33:09 AM com.google.common.base.MoreObjects$ToStringHelper java8CompatibilityCheck
WARNING: Java 7 compatibility warning: See https://github.com/google/guava/issues/5269
java.lang.Exception: Guava will drop support for Java 7 in 2021. Please let us know if this will cause you problems: https://github.com/google/guava/issues/5269
	at com.google.common.base.MoreObjects$ToStringHelper.java8CompatibilityCheck(MoreObjects.java:166)
	at com.google.common.base.MoreObjects$ToStringHelper.<init>(MoreObjects.java:186)
	at com.google.common.base.MoreObjects$ToStringHelper.<init>(MoreObjects.java:146)
	at com.google.common.base.MoreObjects.toStringHelper(MoreObjects.java:111)
	at io.grpc.LoadBalancerProvider.toString(LoadBalancerProvider.java:92)
	at java.lang.String.valueOf(String.java:2849)
	at java.lang.StringBuilder.append(StringBuilder.java:128)
	at io.grpc.LoadBalancerRegistry.getDefaultRegistry(LoadBalancerRegistry.java:109)
	at io.grpc.internal.AutoConfiguredLoadBalancerFactory.<init>(AutoConfiguredLoadBalancerFactory.java:53)
	at io.grpc.internal.ManagedChannelImpl.<init>(ManagedChannelImpl.java:610)
	at io.grpc.internal.ManagedChannelImplBuilder.build(ManagedChannelImplBuilder.java:612)
	at io.grpc.internal.AbstractManagedChannelImplBuilder.build(AbstractManagedChannelImplBuilder.java:261)
	at com.google.api.gax.grpc.testing.LocalChannelProvider.getTransportChannel(LocalChannelProvider.java:136)
	at com.google.api.gax.rpc.ClientContext.create(ClientContext.java:169)
	at com.google.cloud.videointelligence.v1p3beta1.stub.GrpcVideoIntelligenceServiceStub.create(GrpcVideoIntelligenceServiceStub.java:69)
	at com.google.cloud.videointelligence.v1p3beta1.stub.VideoIntelligenceServiceStubSettings.createStub(VideoIntelligenceServiceStubSettings.java:114)
	at com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClient.<init>(VideoIntelligenceServiceClient.java:138)
	at com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClient.create(VideoIntelligenceServiceClient.java:118)
	at com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClientTest.setUp(VideoIntelligenceServiceClientTest.java:76)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:606)
	at org.junit.runners.model.FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:59)
	at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
	at org.junit.runners.model.FrameworkMethod.invokeExplosively(FrameworkMethod.java:56)
	at org.junit.internal.runners.statements.RunBefores.invokeMethod(RunBefores.java:33)
	at org.junit.internal.runners.statements.RunBefores.evaluate(RunBefores.java:24)
	at org.junit.internal.runners.statements.RunAfters.evaluate(RunAfters.java:27)
	at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
	at org.junit.runners.BlockJUnit4ClassRunner$1.evaluate(BlockJUnit4ClassRunner.java:100)
	at org.junit.runners.ParentRunner.runLeaf(ParentRunner.java:366)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:103)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:63)
	at org.junit.runners.ParentRunner$4.run(ParentRunner.java:331)
	at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:79)
	at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:329)
	at org.junit.runners.ParentRunner.access$100(ParentRunner.java:66)
	at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:293)
	at org.junit.internal.runners.statements.RunBefores.evaluate(RunBefores.java:26)
	at org.junit.internal.runners.statements.RunAfters.evaluate(RunAfters.java:27)
	at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
	at org.junit.runners.ParentRunner.run(ParentRunner.java:413)
	at org.junit.runners.Suite.runChild(Suite.java:128)
	at org.junit.runners.Suite.runChild(Suite.java:27)
	at org.junit.runners.ParentRunner$4.run(ParentRunner.java:331)
	at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:79)
	at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:329)
	at org.junit.runners.ParentRunner.access$100(ParentRunner.java:66)
	at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:293)
	at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
	at org.junit.runners.ParentRunner.run(ParentRunner.java:413)
	at org.apache.maven.surefire.junitcore.JUnitCore.run(JUnitCore.java:55)
	at org.apache.maven.surefire.junitcore.JUnitCoreWrapper.createRequestAndRun(JUnitCoreWrapper.java:137)
	at org.apache.maven.surefire.junitcore.JUnitCoreWrapper.executeEager(JUnitCoreWrapper.java:107)
	at org.apache.maven.surefire.junitcore.JUnitCoreWrapper.execute(JUnitCoreWrapper.java:83)
	at org.apache.maven.surefire.junitcore.JUnitCoreWrapper.execute(JUnitCoreWrapper.java:75)
	at org.apache.maven.surefire.junitcore.JUnitCoreProvider.invoke(JUnitCoreProvider.java:157)
	at org.apache.maven.surefire.booter.ForkedBooter.runSuitesInProcess(ForkedBooter.java:428)
	at org.apache.maven.surefire.booter.ForkedBooter.execute(ForkedBooter.java:162)
	at org.apache.maven.surefire.booter.ForkedBooter.run(ForkedBooter.java:562)
	at org.apache.maven.surefire.booter.ForkedBooter.main(ForkedBooter.java:548)
Caused by: java.lang.UnsupportedClassVersionError: com/google/common/base/Java8Usage : Unsupported major.minor version 52.0
	at java.lang.ClassLoader.defineClass1(Native Method)
	at java.lang.ClassLoader.defineClass(ClassLoader.java:803)
	at java.security.SecureClassLoader.defineClass(SecureClassLoader.java:142)
	at java.net.URLClassLoader.defineClass(URLClassLoader.java:442)
	at java.net.URLClassLoader.access$100(URLClassLoader.java:64)
	at java.net.URLClassLoader$1.run(URLClassLoader.java:354)
	at java.net.URLClassLoader$1.run(URLClassLoader.java:348)
	at java.security.AccessController.doPrivileged(Native Method)
	at java.net.URLClassLoader.findClass(URLClassLoader.java:347)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:425)
	at sun.misc.Launcher$AppClassLoader.loadClass(Launcher.java:312)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:358)
	at com.google.common.base.MoreObjects$ToStringHelper.java8CompatibilityCheck(MoreObjects.java:164)
	... 61 more

[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 2.115 s - in com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClientTest
[INFO] Running com.google.cloud.videointelligence.v1p3beta1.StreamingVideoIntelligenceServiceClientTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.059 s - in com.google.cloud.videointelligence.v1p3beta1.StreamingVideoIntelligenceServiceClientTest
[INFO] Running com.google.cloud.videointelligence.v1.VideoIntelligenceServiceClientTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.105 s - in com.google.cloud.videointelligence.v1.VideoIntelligenceServiceClientTest
[INFO] Running com.google.cloud.videointelligence.v1beta2.VideoIntelligenceServiceClientTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.086 s - in com.google.cloud.videointelligence.v1beta2.VideoIntelligenceServiceClientTest
[INFO] Running com.google.cloud.videointelligence.v1p2beta1.VideoIntelligenceServiceClientTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.092 s - in com.google.cloud.videointelligence.v1p2beta1.VideoIntelligenceServiceClientTest
[INFO] Running com.google.cloud.videointelligence.v1p1beta1.VideoIntelligenceServiceClientTest
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.055 s - in com.google.cloud.videointelligence.v1p1beta1.VideoIntelligenceServiceClientTest
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 12, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence ---
[INFO] Loading execution data file /tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence/target/jacoco.exec
[INFO] Analyzed bundle 'Google Cloud Video Intelligence' with 48 classes
[INFO] 
[INFO] --------< com.google.cloud:google-cloud-video-intelligence-bom >--------
[INFO] Building Google Cloud video-intelligence BOM 1.5.9               [13/13]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] --- maven-enforcer-plugin:3.0.0-M3:enforce (enforce) @ google-cloud-video-intelligence-bom ---
[INFO] Skipping Rule Enforcement.
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:prepare-agent (default) @ google-cloud-video-intelligence-bom ---
[INFO] argLine set to -javaagent:/root/.m2/repository/org/jacoco/org.jacoco.agent/0.8.6/org.jacoco.agent-0.8.6-runtime.jar=destfile=/tmpfs/src/github/java-video-intelligence/google-cloud-video-intelligence-bom/target/jacoco.exec
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-resource (add-main-proto-resources) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] --- build-helper-maven-plugin:3.2.0:add-test-resource (add-test-proto-resources) @ google-cloud-video-intelligence-bom ---
[INFO] 
[INFO] --- jacoco-maven-plugin:0.8.6:report (report) @ google-cloud-video-intelligence-bom ---
[INFO] Skipping JaCoCo execution due to missing execution data file.
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO] 
[INFO] Google Cloud Video Intelligence Parent 1.5.9 ....... SUCCESS [  1.397 s]
[INFO] proto-google-cloud-video-intelligence-v1p3beta1 0.87.9 SUCCESS [  1.282 s]
[INFO] proto-google-cloud-video-intelligence-v1beta2 0.87.9 SUCCESS [  0.109 s]
[INFO] proto-google-cloud-video-intelligence-v1p1beta1 0.87.9 SUCCESS [  0.232 s]
[INFO] proto-google-cloud-video-intelligence-v1 1.5.9 ..... SUCCESS [  0.255 s]
[INFO] proto-google-cloud-video-intelligence-v1p2beta1 0.87.9 SUCCESS [  0.153 s]
[INFO] grpc-google-cloud-video-intelligence-v1p1beta1 0.87.9 SUCCESS [  0.259 s]
[INFO] grpc-google-cloud-video-intelligence-v1beta2 0.87.9  SUCCESS [  0.101 s]
[INFO] grpc-google-cloud-video-intelligence-v1 1.5.9 ...... SUCCESS [  0.109 s]
[INFO] grpc-google-cloud-video-intelligence-v1p2beta1 0.87.9 SUCCESS [  0.091 s]
[INFO] grpc-google-cloud-video-intelligence-v1p3beta1 0.87.9 SUCCESS [  0.089 s]
[INFO] Google Cloud Video Intelligence 1.5.9 .............. SUCCESS [  7.804 s]
[INFO] Google Cloud video-intelligence BOM 1.5.9 .......... SUCCESS [  0.044 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  13.403 s
[INFO] Finished at: 2021-02-19T10:33:12Z
[INFO] ------------------------------------------------------------------------
coercing sponge logs...
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1.VideoIntelligenceServiceClientTest-sponge_log.xml
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1p3beta1.StreamingVideoIntelligenceServiceClientTest-sponge_log.xml
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1p3beta1.VideoIntelligenceServiceClientTest-sponge_log.xml
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1p2beta1.VideoIntelligenceServiceClientTest-sponge_log.xml
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1beta2.VideoIntelligenceServiceClientTest-sponge_log.xml
processing ./google-cloud-video-intelligence/target/surefire-reports/TEST-com.google.cloud.videointelligence.v1p1beta1.VideoIntelligenceServiceClientTest-sponge_log.xml
exiting with 0
cleanup


[ID: 7364974] Build finished after 96 secs, exit value: 0


Warning: Permanently added 'localhost' (ECDSA) to the list of known hosts.
[02:33:13] Collecting build artifacts from build VM
[02:33:15] Kokoro builder finished
