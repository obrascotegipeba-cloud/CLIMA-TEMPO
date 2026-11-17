# Alerta de Chuva (Android)

App com os mesmos parâmetros da planilha e tela no estilo Google Clima (faixa de horas, cartões dos dias e tabela 15 dias × 24 h): cidade, UF, chance mínima (%) e chuva mínima (mm).
Verifica a previsão a cada 3 horas em segundo plano e toca um **alarme sonoro** (repete até você tocar
na notificação) quando há previsão de chuva para o **dia seguinte**. Toca uma vez por dia previsto.
Dados: Open-Meteo (gratuito, sem cadastro). Android 8.0 ou mais novo.

## Opção A – Gerar o APK no GitHub (sem instalar nada)
1. Crie uma conta em github.com e um repositório novo (pode ser privado).
2. Clique em "uploading an existing file" e arraste TODO o conteúdo desta pasta
   (inclusive a pasta `.github`). Clique em "Commit changes".
3. Abra a aba **Actions** do repositório. O processo "Gerar APK" roda sozinho (uns 5 minutos).
4. Quando ficar verde, clique nele e baixe **AlertaChuva-apk** (vem em .zip; dentro está o `app-debug.apk`).
5. Passe o .apk para o celular e instale (o Android pede para permitir "instalar apps desconhecidos").

## Opção B – Android Studio
1. Instale o Android Studio (developer.android.com/studio).
2. File > Open > selecione esta pasta. Aguarde a sincronização.
3. Build > Build App Bundle(s) / APK(s) > Build APK(s).
4. O APK fica em `app/build/outputs/apk/debug/app-debug.apk`.

## No celular
- Abra o app, digite a cidade, escolha a UF, ajuste os limites e toque em **Salvar e verificar agora**.
- Permita as notificações quando o Android pedir.
- Toque em **Testar som do alerta** para ouvir o alarme.
- Em alguns aparelhos (Xiaomi, Samsung, Motorola), libere o app em
  Configurações > Bateria > "Sem restrições", senão o sistema pode bloquear a verificação em segundo plano.

## Tela
A tela fica em `app/src/main/assets/index.html` (mesmo visual da página de previsão hora a hora).
Abrindo esse arquivo no navegador do computador dá para ver uma demonstração com dados de Cotegipe.
