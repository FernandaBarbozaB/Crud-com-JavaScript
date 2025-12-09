🌟 CRUD Completo em JavaScript

✨ Funcionalidades

* Criar novos registros através de um formulário intuitivo.
* Exibir os dados em uma tabela dinâmica.
* Editar qualquer registro com facilidade.
* Excluir itens com um clique.
* Renderização imediata a cada mudança no estado dos dados.

---

## 🔧 Arquitetura do Projeto

* **HTML** — Estrutura organizada.
* **CSS** — Estilo leve e funcional.
* **JavaScript** — Toda a lógica e manipulação.

Sem frameworks. Sem dependências externas. Apenas o essencial — bem construído.

---

## Como o Projeto Funciona

### 1. Criar (Create)

O usuário preenche um formulário, o JavaScript captura esses valores e cria um objeto que é inserido em um array.

### 2. Ler (Read)

A função de renderização percorre o array e insere dinamicamente cada registro na tabela.

### 3. Atualizar (Update)

Ao clicar em "editar", os dados são enviados de volta ao formulário. Após confirmar, o item correspondente é atualizado no array e a tabela é redesenhada.

### 4. Deletar (Delete)

Com um clique, o registro é removido do array e a tabela é atualizada.

---

## 📂 Estrutura de Pastas

```
/projeto-crud
│── index.html
│── style.css
└── script.js
```

---

## 🏃‍♀️ Como Rodar Localmente

### 🔹 Método 1 — Abrindo direto no navegador

1. Baixe ou clone o repositório:

  git clone https://github.com/FernandaBarbozaB/Crud-com-JavaScript.git

ou

2. Abra a pasta do projeto.
3. Execute o arquivo **index.html** (clique duplo ou abrir no navegador).

### 🔹 Método 2 — Rodar com Live Server 
1. Abra o projeto no **VS Code**.
2. Instale a extensão **Live Server**.
3. Clique com o botão direito no arquivo `index.html`.
4. Escolha **Open with Live Server**.

O navegador abrirá em:
```

[http://127.0.0.1:5500/](http://127.0.0.1:5500/)

```
Com recarregamento automático a cada alteração.

---

🌱 Este projeto utiliza o localStorage do navegador como estratégia de persistência de dados no front-end. 

Em vez de depender de um banco de dados externo, a aplicação armazena os registros localmente no próprio browser, permitindo que as informações permaneçam salvas mesmo após o fechamento ou recarregamento da página.

O funcionamento ocorre da seguinte forma:

Os dados são mantidos em uma estrutura de array em JavaScript.

Sempre que um item é criado, editado ou removido, o estado completo desse array é convertido em JSON utilizando JSON.stringify().

Esse JSON é então armazenado no navegador através de localStorage.setItem().

Quando o usuário acessa novamente a aplicação:

O sistema verifica se já existem dados salvos.

Caso existam, eles são recuperados via localStorage.getItem() e convertidos de volta para objetos JavaScript com JSON.parse().

A interface é automaticamente reconstruída com base nesses dados persistidos.

Essa abordagem demonstra domínio de:

✅ Persistência de dados no front-end
✅ Manipulação de estado da aplicação
✅ Serialização e desserialização de objetos com JSON
✅ Boas práticas em aplicações sem backend


