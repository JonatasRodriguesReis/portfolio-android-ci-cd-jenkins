## Android set up

export KEYSTORE_FILE=$(pwd)/release.keystore
export KEYSTORE_PASSWORD=senha_do_keystore
export KEY_ALIAS=ciappkey
export KEY_PASSWORD=senha_da_key

./gradlew assembleRelease
