## Android set up

export KEYSTORE_FILE=$(pwd)/release.keystore
export KEYSTORE_PASSWORD=senha_do_keystore
export KEY_ALIAS=ciappkey
export KEY_PASSWORD=senha_da_key

./gradlew assembleRelease

“O Jenkins gera o APK assinado e publica automaticamente no Firebase App Distribution usando uma service account, permitindo testes internos sem Play Store.”
