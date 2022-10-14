---
description: RTFM
---

# 🛠 Configurar

Se acontecer algum erro, verifique o [FAQ](faq.md).

Antes de começar, verifique se ativou a visibilidade do Status de Atividade nas definições do Discord:

<figure><img src="https://user-images.githubusercontent.com/63465951/195862088-05f85566-77fa-4654-a62a-faeaee538a46.jpg" alt=""><figcaption></figcaption></figure>

## Setup process

* Vá a https://discord.com/developers/applications/.
* Clique em **New Application** no canto superior direito.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Escolha um nome para a aplicação, este irá aparecer após o A Jogar: no status; Clique em **Create**.
* Copie o **Application ID** e cole-o na barra do CustomRP **ID**, e clique em **Conectar**. Se isto for feito corretamente, o seu status no Discord deve aparecer como "Jogando **\[nome do app]**".
  * Nota: Se tiveres o teu status customizado ativado (o que tem os emojis), vai ser periorizado em vez do CustomRP. Mas vai ser visto no seu perfil de qualquer forma.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

  * Na sua página de aplicações, navegue para Rich Presence -> Art Assets e faça upload de pelo menos uma imagem que voçê queira usar. No CustomRP existe um botão de **Carregar Imagens** no menu de Ficheiros (também pode ser acessado ao clicar em Ctrl+U), isto irá leva-lo para lá se a barra de ID estiver preenchida corretamente.
  * Alternativamente, pode simplesmente adicionar um Link para a imagem na sua respetiva barra.
  * Nota: Enquanto você pode chamar a sua imagem até 999 caracteres, a API irá apenas aceitar no máximo 256.
* Navegue para o **Visualizer** e insira o que quiser nas barras **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. Todos eles são opcionais.
* Após terminar de configurar a Presença ao seu gosto copie-os para as barras correspondentes no CustomRP.
  * Dica: Pode por o rato em cima de quase qualquer coisa na aplicação (incluindo a palavra **Details**) e vai-te aparecer o que ele faz!
* Se também quiser configurar os botões, preencha as barras de **Botão** e **URL**.
  * Nota: Quando você clicar nos botões da sua própria presença, eles não vão funcionar, mas não se preocupe pois eles irão funcionar para toda a gente. É apenas um problema com o Discord.
* Clique em **Atualizar Presença** (ou **Conectar** se já não estiver conectado).
* E parabéns!, Você agora é incrível!

### Eu uso mais que um cliente do Discord, o que eu faço?

Se você tiver mais que um cliente do Discord e gostaria que a presença aparecesse diferente de uma conta para a outra, clique em **Disconectar**, e prima Ctrl+Shift no seu teclado e clique em **Conectar**. Uma janela com um número irá aparecer, insira o número 1, feche a janela e clique em **Conectar** outra vez, sem premir Ctrl+Shift. Caso seja uma conta inválida, tente o número 0, depois 2 até 9.

Por favor tenha em atenção que ter vários clientes do Discord a abrir ao iniciar do windows, o número da "Pipe" para cada cliente pode não ser sempre o mesmo e pode trocar dependendo do cliente que abriu primeiro. Para resolver isso, você pode abri-los manualmente ou usar o "Programador de Tarefas" do Windows para atrasar a abertura de clientes.

Se você tiver 2 contas que você use ao mesmo tempo e gostaria que cada uma delas tivesse uma presença diferente então siga estes passos:

* Prepare a sua conta principal primeiro com as instruções indicadas acima.
* Transfira a última versão do **portable (.zip)** do CustomRP (tanto do website [Website](https://www.customrp.xyz) ou [A Página do GitHub](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) e deszipeo em qualquer lado.
  * Isto apenas funciona na versão 1.16+.
* Abra `Start Second Instance.bat` ou crie um atalho do CustomRP.exe com o argumento `--second-instance` (ou `-2`).
* Configure o programa da mesma forma que você configurou a sua instância principal mas com as mudanças que você quiser.
  * Dica: Se você já tiver um preset e gostaria de o usar com a sua segunda instância, você pode editar o ficheiro .bat ou o atalho para incluir o endereço do preset. Exemplo: `CustomRP.exe -2 "C:\PresetsFixes\preset.crp"` (aspas ao redor do caminho são necessárias se o caminho tiver espaços nele).
* Antes de conectar, mude a "Pipe" como descrito antes e conecte.

Se você usar 3 ou mais contas ao mesmo tempo... porquê? Mas se várias pessoas me vierem chatear a cabeça, eu posso adicionar suporte para mais instâncias.

## Notas

* Se você não quiser configurar uma imagem grande ou pequena, deixe essas barras brancas.
* Se a imagem grande não estiver configurada, as definições da imagem pequena serão ignoradas.
