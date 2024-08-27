# Python S3 Backup Script
## Descrição:

Este script Python oferece uma solução robusta para automatizar o backup de arquivos de uma pasta local para um bucket no Amazon S3. Ele garante a segurança dos seus dados, lidando com a listagem de arquivos, upload para o S3 e a exclusão segura dos arquivos locais após o processo.

## Funcionalidades:

* **Configuração via .env:** Mantém suas credenciais AWS e configurações de bucket seguras e organizadas em um arquivo .env.
* **Listagem de arquivos:** Lista todos os arquivos dentro da pasta local especificada, preparando-os para o upload.
* **Upload para o S3:** Utiliza o Boto3 para fazer o upload eficiente dos arquivos para o bucket S3 definido.
* **Exclusão local:** Após o upload bem-sucedido, remove os arquivos da pasta local, economizando espaço em disco.
* **Tratamento de erros:** Implementa um tratamento de erros abrangente para garantir a robustez do script e fornecer mensagens claras em caso de falhas.

## Como usar:

### 1. Clone o repositório:

```Bash
git clone https://github.com/seu-usuario/python-s3-backup.git
cd python-s3-backup
```

### 2. Crie o arquivo .env:

```Bash
touch .env
```

### 3. Preencha o .env com suas credenciais:
```
AWS_ACCESS_KEY_ID=SUA_CHAVE_DE_ACESSO
AWS_SECRET_ACCESS_KEY=SUA_CHAVE_SECRETA
AWS_REGION=SUA_REGIÃO_AWS (ex: us-east-1)
BUCKET_NAME=NOME_DO_SEU_BUCKET_S3
```

### 4. Instale as dependências:

```Bash
pip install boto3 python-dotenv
```

### 5. Execute o script:

```Bash
python seu_script.py
```

### Observações:

* Substitua 'download' pelo caminho da sua pasta local no script.
* Certifique-se de que suas credenciais AWS tenham permissão para acessar o bucket S3.
* Este script é um exemplo e pode ser personalizado para atender às suas necessidades específicas.

### Contribuições:

Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request com melhorias ou correções.
