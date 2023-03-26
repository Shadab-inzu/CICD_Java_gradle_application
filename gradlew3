#!/usr/bin/env sh

##############################################################################
##
##  Gradle start up script for UN*X
##
##############################################################################

# Set environment variables for Gradle
export GRADLE_OPTS="--add-opens=java.base/java.lang=ALL-UNNAMED --illegal-access=warn"

# Resolve the location of the real script, even if it's a symlink
PRG="$0"
while [ -h "$PRG" ] ; do
    ls=`ls -ld "$PRG"`
    link=`expr "$ls" : '.*-> \(.*\)$'`
    if expr "$link" : '/.*' > /dev/null; then
        PRG="$link"
    else
        PRG=`dirname "$PRG"`"/$link"
    fi
done

# Set the script's directory as the current directory
SAVED="`pwd`"
cd "`dirname \"$PRG\"`/" >/dev/null

# Set the location of the Gradle wrapper
export GRADLE_HOME=`pwd`/.gradle/wrapper/dists/gradle-8.0-bin/2osvnnl79t40h28jbap0rbnrvp/gradle-8.0-bin

# Run the Gradle wrapper with the given arguments
"./gradle/wrapper/bin/gradle" "$@"

# Return to the original directory
cd "$SAVED" >/dev/null

exit 0