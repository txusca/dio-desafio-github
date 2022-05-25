# Anotações relacionadas ao SSH na configuração do Git com o GitHub 📋🔒

1 - Necessidade de criação da chave com o comando `ssh-keygen -t ed25519 -C email@email.com`, para que seja gerado a chave pública e privada que será utilizada no github.

2 - Abrir as configurações do GitHub e colocar a chave remota na aba SSH keys a chave gerada.

3 - É necessário a inicialização do processo do `ssh-agent` para utilizar a chave local na máquina em questão, utilizando o comando `eval "$(ssh-agent -s)"`, em seguida adicionando a chave por meio do processo já aberto com o comando `ssh-add ./localchave`.