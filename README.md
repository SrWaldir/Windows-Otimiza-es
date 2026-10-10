# Windows-Otimizacoes
Comandos e ajustes em Windows 10/11 que desativados, consomem menos RAM e CPU, além de resultar em velocidade e fluidez.

1. Ajustes no MSConfig e Serviços
* **Atalho:** Pressione `WIN + R`, digite `msconfig` e dê Enter.
* **Serviços:** Na aba **Serviços**, marque a caixa *"Ocultar todos os serviços da Microsoft"* e desative updaters e programas desnecessários de terceiros (ex: atualizadores de programas, Epic, Adobe, etc.) que iniciam com o Windows.
* **Nota sobre Processadores:** Deixe a opção de número de núcleos no MSConfig **desmarcada**. O Windows gerencia todos os núcleos nativamente de forma dinâmica. Forçar isso manualmente serve apenas para restrição de hardware.

2. Plano de Energia de Desempenho Máximo.
1. Abra o Painel de Controle > Opções de Energia.
2. Altere para o plano de **Alto Desempenho** (ou ative o plano oculto de *Desempenho Máximo* via PowerShell se necessário).

3. Limpeza de Arquivos Temporários e Cache.
Abra o Executar (`WIN + R`) e limpe o conteúdo das seguintes pastas:
* `temp` (Arquivos temporários do sistema)
* `%temp%` (Arquivos temporários do usuário)
* `prefetch` (Cache de pré-carregamento do sistema)
*(Dica: Se algum arquivo recusar exclusão por estar em uso, basta ignorar).*

4. Limpeza de Disco e Otimização.
* Abra o menu Iniciar, digite **Desfragmentar e Otimizar Unidades**.
* Execute a otimização nas suas unidades (mantém o SSD/HD organizado e saudável).
* Use a **Limpeza de Disco** nativa para remover arquivos de instalação anteriores do Windows (`Windows.old`) e arquivos de atualização.

5. Redução de Efeitos Visuais.
1. Pressione `WIN + R`, digite `sysdm.cpl` e vá na aba **Avançado**.
2. Em **Desempenho**, clique em **Configurações**.
3. Selecione *"Ajustar para obter o melhor desempenho"* (ou desmarque animações excessivas para manter a interface limpa e rápida).

6. Remoção de Apps e Inicialização
* **Gerenciador de Tarefas (`Ctrl + Shift + Esc`):** Vá na aba **Aplicativos de Inicialização** e desative tudo o que não precisa abrir junto com o Windows (OneDrive, Skype, Discord, etc.).
* **Desinstalação de Apps Nativos:** Remova aplicativos pré-instalados da Microsoft que você nunca usa (Paint 3D, Cortana, OneDrive, etc.).
