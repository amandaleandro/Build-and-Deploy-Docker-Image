# Build and Deploy Docker Image

## Descrição
Este projeto consiste em uma automação para construir uma imagem Docker de uma aplicação e implantá-la em um servidor Droplet. É útil para simplificar o processo de construção e implantação de aplicações Docker em ambientes de produção.

## Pré-requisitos
- Acesso a um repositório Git hospedado no GitHub.
- Um Droplet configurado e acessível via SSH.
- Credenciais de acesso ao Droplet, como nome de usuário e chave SSH.

## Configuração
1. Clone este repositório para o seu ambiente de desenvolvimento.
2. Certifique-se de ter o Docker instalado e funcionando localmente.
3. Configure as variáveis de ambiente secretas no GitHub:
    - `DROPLET_HOST`: O endereço IP ou o nome de domínio do seu Droplet.
    - `DROPLET_USERNAME`: Seu nome de usuário no Droplet.
    - `DROPLET_SSH_KEY`: Sua chave SSH privada para acessar o Droplet.
4. Personalize o arquivo Dockerfile dentro do diretório `my-app` para incluir as dependências e configurações necessárias para sua aplicação.
5. Modifique conforme necessário o caminho do diretório ou o nome da imagem Docker no arquivo de fluxo de trabalho `.yml`.

## Uso
1. Faça as alterações desejadas na sua aplicação.
2. Faça o commit e o push das suas alterações para o branch `main`.
3. O GitHub Actions será acionado automaticamente, construindo a nova imagem Docker e implantando-a no seu Droplet.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas ou enviar pull requests para melhorar este projeto.

## Licença
Este projeto é licenciado sob a MIT License. Consulte o arquivo LICENSE para obter mais detalhes.