# Página de Login para Campanhas de Phishing e Conscientização

Este repositório contém um código HTML utilizado para simulações de phishing e campanhas de conscientização de segurança. Ele é projetado para ser usado por pesquisadores de segurança e equipes de Red Team com o intuito de testar a conscientização de usuários e a eficácia de medidas de segurança contra ataques de phishing.

## Descrição

![image](https://github.com/user-attachments/assets/3a429fc8-3aa2-4437-b653-f959a50a6f09)

A página imita uma tela de login que pode ser configurada para parecer com diferentes sites ou serviços. O formulário de login coleta as informações do usuário (como nome de usuário e senha) e, ao ser submetido, envia esses dados junto com informações de geolocalização e IP para um webhook do Discord. A coleta de dados de login e informações de localização pode ser útil para campanhas de conscientização e testes de segurança.

**Atenção:** Este código é fornecido exclusivamente para fins educacionais, testes e simulações de segurança. O uso não autorizado deste código é ilegal e pode resultar em sérias consequências legais.

## Vantagens

Com uma pagina dedicada você pode hospedar o site e deixa-lo aberto por quanto tempo quiser sem precisar subir o serviço com a sua maquina pessoal ou a necessidade de uma VPS para deixar online o tempo todo. Alem disso, por se um simples index você pode implementa-lo dentro de aplicações reais ou abusar de **CSRF**, **SSRF** ou **Clickjacking**

## Funcionalidades

- **Formulário de Login**: A página contém um formulário de login com campos para nome de usuário e senha.
- **Mensagem de Erro**: Se as credenciais fornecidas forem inválidas, uma mensagem de erro é exibida.
- **Envio de Dados**: Quando o formulário é enviado, ele coleta dados como nome de usuário, senha, e informações do IP, como cidade, região e ISP.
- **Webhook do Discord**: Os dados coletados são enviados para um webhook do Discord em formato de embed.
- **Alteração de Idioma**: A página permite a troca entre diferentes idiomas (Português, Inglês e Espanhol).
- **Estilo Personalizado**: A página conta com um design simples e responsivo, otimizado para diferentes dispositivos.

## Como Funciona

1. O usuário preenche o formulário de login com nome de usuário e senha.
2. Ao enviar o formulário, o código JavaScript captura as informações inseridas e obtém dados de geolocalização através da API `ipinfo.io`.
3. A informação é enviada via um webhook para o Discord, onde os dados aparecem como uma mensagem com as credenciais do usuário e a localização.

![Captura de tela 2025-02-03 145225](https://github.com/user-attachments/assets/186927c7-f9bd-410a-a677-aa8ec33e3b7b)

## Como Usar

### Pré-requisitos

- Nenhum servidor especial é necessário. Basta hospedar o arquivo HTML em um servidor web ou localmente.
- **Webhook do Discord**: Você precisará de um webhook do Discord para enviar os dados. O URL do webhook é configurado no código.

### Passos para Implementação

1. Clone ou baixe o repositório.
2. Abra o arquivo HTML e edite o URL do webhook no script (substitua pelo seu próprio URL de webhook do Discord).
3. Abra a página em um navegador para visualizar e testar a página de login.
4. Para realizar testes, use um servidor local (como `http-server` ou qualquer outro servidor web simples).
5. Use a página para simulações de phishing ou treinamento de conscientização.

## Personalização

Você pode personalizar a página de login para imitar qualquer serviço online. A imagem do logo e as mensagens podem ser alteradas facilmente editando o HTML.

## Aviso Legal

**Uso Ético**: Este código foi desenvolvido para fins educativos, e simulações controladas. **Nunca utilize este código para atividades ilegais** ou sem o consentimento explícito da vítima. O uso de técnicas de phishing para enganar ou prejudicar outros é contra a lei.

## Contribuições

Se você quiser contribuir com melhorias ou sugestões, sinta-se à vontade para abrir uma issue ou enviar um pull request. Lembre-se de manter o foco na segurança e no uso ético deste projeto.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE), o que permite o uso e modificação do código de acordo com os termos da licença.
