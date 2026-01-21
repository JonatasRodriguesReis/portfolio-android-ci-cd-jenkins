## Android set up

export KEYSTORE_FILE=$(pwd)/release.keystore
export KEYSTORE_PASSWORD=senha_do_keystore
export KEY_ALIAS=ciappkey
export KEY_PASSWORD=senha_da_key

./gradlew assembleRelease

“O Jenkins gera o APK assinado e publica automaticamente no Firebase App Distribution usando uma service account, permitindo testes internos sem Play Store.”
“Implementei observabilidade no pipeline com métricas, logs centralizados e dashboards para acompanhar builds, falhas e duração.”
“Estruturei o projeto para ser totalmente reproduzível, com observabilidade definida como código usando Docker Compose, Prometheus, Grafana e Loki, permitindo deploy local ou em cloud sem dependência de provedor.”
“Separei CI e observabilidade em docker-composes distintos, conectados por uma network externa, e utilizei Promtail para coleta de logs, garantindo comunicação e observabilidade de forma cloud-agnostic.”
“Configurei o pipeline para interromper a distribuição automaticamente caso qualquer etapa anterior falhe, garantindo qualidade e rastreabilidade.”
“Criei uma imagem customizada do Jenkins para garantir todas as dependências de build, evitando falhas por comandos ausentes e tornando o pipeline totalmente reprodutível.”
