
# Installing NVM with Homebrew on macOS

## Passo 1: Abrir o Terminal
Abra o **Terminal** no seu sistema macOS.

---

## Passo 2: Instalar o Homebrew
Certifique-se de que o **Homebrew** está instalado.  
Se não estiver, instale-o usando o comando:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

## Passo 3: Atualizar o Homebrew
Atualize o Homebrew para a versão mais recente executando:

```bash
brew update
```

---

## Passo 4: Instalar o NVM
Instale o **NVM** usando o Homebrew:

```bash
brew install nvm
```

---

## Passo 5: Criar diretório para o NVM
Crie um diretório para o NVM na sua pasta pessoal:

```bash
mkdir ~/.nvm
```

---

## Passo 6: Configurar variáveis de ambiente
Edite o arquivo de configuração do seu shell:

- Para **zsh** (macOS Catalina ou posterior):  
  ```bash
  vim ~/.zshrc
  ```
- Para **bash**:  
  ```bash
  vim ~/.bash_profile
  ```

Adicione as seguintes linhas ao arquivo:

```bash
export NVM_DIR="$HOME/.nvm"
[ -s "$(brew --prefix nvm)/nvm.sh" ] && \. "$(brew --prefix nvm)/nvm.sh"
```

Salve e feche o arquivo pressionando `ESC`, digitando `:wq` e pressionando **Enter**.

---

## Passo 7: Carregar variáveis de ambiente
Carregue as variáveis de ambiente atualizadas na sessão atual do shell:

```bash
source ~/.zshrc
```

---

## Passo 8: Verificar instalação
Verifique a instalação conferindo a versão do NVM:

```bash
nvm --version
```
```

Quer que eu também formate isso em um **guia passo a passo com checklist** (✅) para ficar ainda mais didático?
