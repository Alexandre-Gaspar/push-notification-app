# Test Push Notification App

Um aplicativo Android simples para testar notificações push usando Firebase Cloud Messaging (FCM).

## O que o app faz

- Obtém automaticamente o token FCM do dispositivo
- Exibe o token na tela para fácil acesso
- Recebe e exibe notificações push
- Permite copiar o token para área de transferência

## Configuração básica

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com)
2. Adicione um app Android com o package `com.testpushnotificationapp`
3. Baixe o arquivo `google-services.json` e coloque na pasta `app/`. Att: apague o que estiver no projecto e substitua pelo seu.
4. Execute o projeto no Android Studio

## Como testar

1. Execute o app e copie o token exibido
2. Use o token para enviar notificações via:
   - Firebase Console (Cloud Messaging)
   - Sua própria API REST
   - Ferramenta de teste FCM

## Estrutura do projeto

- `TokenScreeen` - Interface principal com exibição do token
- `MyFirebaseMessagingService.kt` - Serviço que gerencia mensagens FCM
- `AndroidManifest.xml` - Configurações de permissões e serviços
- `MainActivity.kt` - Classe principal que chama a screen e todos os seerviços necessários

## Requisitos

- Android Studio
- Android 7.0+ (API 24)
- Conexão com internet
- Permissão de notificações
