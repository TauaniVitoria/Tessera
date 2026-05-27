# Calculadora de Métodos Numéricos

Uma aplicação interativa desenvolvida para execução, visualização e estudo prático de métodos numéricos.

---

## Tecnologias Utilizadas

A aplicação utiliza um ecossistema moderno e robusto voltado para a estabilidade, performance e tipagem estrita:

*   **Core:** React 18 + TypeScript (tipagem estrita)
*   **Empacotador & Dev Server:** Vite
*   **Interpretador Matemático:** MathJS (com otimização por cache de compilação de expressões e derivadas)
*   **Estilização & Componentes:** TailwindCSS + Radix UI / Shadcn boilerplate (design premium, responsivo e adaptativo)
*   **Validação & Qualidade:** ESLint (regras estritas) + Vitest (suíte de testes unitários automatizados)

---

## Como Executar o Projeto

Certifique-se de possuir o [Node.js](https://nodejs.org/) instalado em seu sistema operacional.

### 1. Instalar as dependências
```bash
npm install
```

### 2. Rodar o servidor de desenvolvimento
```bash
npm run dev
```
A aplicação abrirá no endereço local fornecido no terminal (geralmente [http://localhost:5173](http://localhost:5173)).

### 3. Executar a suíte de testes
Para validar o motor matemático e os critérios de parada/convergência:
```bash
npm test
```

### 4. Rodar o linter estático
Para assegurar a conformidade de tipagem e boas práticas:
```bash
npm run lint
```

### 5. Compilar o projeto para produção
Para gerar o pacote de build estático final minificado e otimizado na pasta `dist/`:
```bash
npm run build
```

---

## Distribuição e Instalação (Desktop)

A aplicação pode ser compilada como um aplicativo desktop nativo para macOS e Windows utilizando o **Tauri v2**. Os instaladores oficiais são gerados automaticamente pelo pipeline do GitHub Actions.

### macOS (Instalação e Segurança)

Como a aplicação é distribuída de forma independente (sem assinatura digital paga da Apple), o macOS ativará o **Gatekeeper** na primeira execução, o que é o comportamento esperado.

1. **Baixe sempre o instalador no formato `.dmg`** (evite extrair ou rodar pastas `.app` diretamente de arquivos `.zip`, pois o descompactador do macOS corrompe as permissões Unix de execução do binário interno).
2. Dê um duplo clique no arquivo `.dmg` para montá-lo e **arraste o ícone do aplicativo para a pasta Aplicativos (Applications)**.
3. Para abrir pela primeira vez:
   * Clique com o **botão direito** (ou `Control + Clique`) no ícone do aplicativo na pasta Aplicativos.
   * Selecione **Abrir (Open)** no menu de contexto.
   * Um aviso de segurança aparecerá. Clique no botão **Abrir (Open)** para confirmar a execução.
   * Nas execuções seguintes, basta dar o duplo clique normal para abrir o aplicativo.

### Windows
1. Baixe o instalador `.msi` ou `.exe` (NSIS) gerado na Release/Artifacts.
2. Execute o arquivo e siga as instruções na tela para concluir a instalação.