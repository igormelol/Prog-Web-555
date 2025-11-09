
# 📘 **Configuração do Ambiente e Conceitos Básicos em PHP**

Material de estudo consolidado — Módulos I a IV

Este repositório reúne o conteúdo completo dos módulos sobre **introdução ao PHP**, **configuração de ambiente**, **conceitos essenciais**, **história da linguagem**, **instalação de servidor local**, **uso do XAMPP/Apache/MySQL**, **primeiros scripts** e **comparações estruturais entre PHP e JavaScript**.

É um guia para iniciantes que desejam entender como funciona o PHP no lado do servidor e como preparar um ambiente de desenvolvimento profissional.

---

# 📚 **Conteúdo dos Módulos**

---

## ✅ **Módulo I — O que é PHP? História, características e fundamentos**

Este módulo apresenta a base teórica da linguagem PHP, incluindo sua origem, evolução e aplicabilidade.

### **Tópicos principais**

* **O que é PHP**
  Linguagem interpretada, server-side, multiplataforma e de código aberto.


* **História do PHP**
  Criado por Rasmus Lerdorf em 1994 como PHP/FI, evoluiu para Personal Home Page Tools e, em 1997, para PHP: Hypertext Preprocessor.


* **Características da linguagem**

  * Fácil aprendizado
  * Código aberto
  * Alto desempenho
  * Compatível com bancos de dados (MySQL, SQLite, Oracle)
  * Multiplataforma
  * Base do WordPress
  * Grande quantidade de frameworks (Laravel, Symfony, CodeIgniter, Zend)


* **Onde o PHP é usado**

  * Desenvolvimento de sites dinâmicos
  * Aplicações web
  * Criação de plugins e temas WordPress
  * Scripts de linha de comando


---

## ✅ **Módulo II — PHP x JavaScript: Comparativo completo**

O módulo traz uma análise entre PHP e JavaScript com base em critérios técnicos, produtividade e ecossistema.

### **Critérios analisados**

1. Visão geral

   * JS: linguagem full-stack, multiparadigma, popularidade global
   * PHP: linguagem consolidada para back-end


2. Desempenho e velocidade

   * JS (Node.js): assíncrono, non-blocking, rápido
   * PHP: síncrono e mais lento, porém estável


3. Extensibilidade

   * JS: grande número de frameworks (React, Angular, Vue), NPM
   * PHP: integração forte com CMS (WordPress, Drupal), Composer


4. Universalidade

   * JS: pode ser usado no front e no back
   * PHP: back-end apenas


5. Comunidade

   * Ambas com comunidades fortes, grandes empresas usam ambas


6. Curva de aprendizagem

   * PHP: mais fácil de começar
   * JS: exige mais conhecimento inicial


7. Sintaxe

   * JS e PHP compartilham estruturas comuns (arrays, loops, operadores)
   * Diferenças em concatenação, escopo e case-sensitivity


8. Tipos de aplicações indicadas

   * JS: grandes sistemas full-stack, streaming, IoT
   * PHP: CMS, e-commerce, blogs


✅ **Placar final da comparação: PHP 3 x 5 JavaScript**


---

## ✅ **Módulo III — Configuração do Ambiente PHP (XAMPP, Apache, Servidor embutido)**

### **Instalando o ambiente**

* Instalação do XAMPP
* Iniciar serviços Apache e MySQL
* Arquivos devem ser colocados em **htdocs**


### **Primeiro script PHP**

Criação do arquivo `teste.php`:

```php
<?php
echo "Olá, este é meu primeiro script PHP!";
?>
```

Acesso via navegador:
`http://localhost/teste.php`


### **echo vs print**

* **echo**: mais rápido, aceita múltiplos valores
* **print**: retorna 1, aceita apenas um valor


### **Servidor embutido (sem XAMPP)**

```bash
php -S localhost:8000
```



---

## ✅ **Módulo III — phpinfo(), extensões e boas práticas de segurança**

### **O que é phpinfo()**

Mostra todas as configurações do PHP: versão, módulos, limitação de memória, timezone etc.


### **Para que serve**

* Verificar módulos habilitados
* Verificar versão
* Detectar erros de configuração
* Ajustar limites de execução


### **Boas práticas**

* Remover phpinfo.php após uso
* Restringir acesso ao arquivo


---

## ✅ **Módulo IV — Apache, Virtual Hosts, MySQL e execução de arquivos PHP**

### **O que é Apache**

Servidor web open source compatível com PHP, Python e outras linguagens.


### **Funções do Apache**

* Interpretar requisições HTTP
* Retornar páginas ao navegador
* Suporte a SSL, módulos e alta personalização


### **Criando Virtual Hosts**

Permite simular “vários domínios” no ambiente local.

Exemplo:

```apache
<VirtualHost *:80>
   ServerName www.meuprojeto.com.br
   DocumentRoot "C:\xampp\htdocs\meuprojeto"
</VirtualHost>
```

Necessário editar o arquivo **hosts**:

```
127.0.0.1 www.meuprojeto.com.br
```



### **MySQL**

* Banco de dados relacional
* Multiplataforma
* Usado por Facebook, Twitter, YouTube, Google


