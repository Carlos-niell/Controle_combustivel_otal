# 🏍️ Controle de Combustível e Rotas

Uma aplicação robusta e responsiva (PWA) desenvolvida em **Oracle APEX** para a gestão eficiente de turnos, acompanhamento de quilometragem e controle de despesas com combustível para motoboys.

![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge)
![Versão](https://img.shields.io/badge/Vers%C3%A3o-1.0-blue?style=for-the-badge)

## 🛠️ Tecnologias Utilizadas

![Oracle Database](https://img.shields.io/badge/Oracle_DB-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Oracle APEX](https://img.shields.io/badge/Oracle_APEX-333333?style=for-the-badge&logo=oracle&logoColor=white)
![PL/SQL](https://img.shields.io/badge/PL/SQL-00758F?style=for-the-badge&logo=database&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5/CSS3](https://img.shields.io/badge/HTML5_/_CSS3-E34F26?style=for-the-badge&logo=html5&logoColor=white)

## ✨ Principais Funcionalidades

- **📊 Dashboard Dinâmico (Painel Geral):** Visualização em tempo real de KM rodados, total abastecido, custos gerados no dia e um alerta inteligente de segurança contra pane seca.
- **⏱️ Gestão de Turnos:** Abertura e encerramento de rotas diárias de forma simples, validando automaticamente a quilometragem inicial e final com base no último turno registado.
- **⛽ Registo de Abastecimentos:** Formulário com cálculos automáticos em JavaScript (preço por litro, distância até ao posto) e upload/download de fotos dos comprovativos (talões).
- **🛣️ Leitura Rápida de Odómetro:** Lógica de entrada rápida com apenas os 3 últimos dígitos do painel. O sistema calcula automaticamente o total acumulado gerindo as viragens de kms (Módulo 1000).
- **🔐 Segurança e Controlo de Acessos:** Controlo total baseado em perfis (Administrador, Contribuidor, Leitor) utilizando a ACL nativa do Oracle APEX.

## 📱 Estrutura da Aplicação

1. **Home (`Página 1`):** Visão executiva com cartões de métricas, histórico de turnos e lista dos últimos abastecimentos. Possui botão rápido de encerramento de turno.
2. **Abertura de Turno (`Página 2`):** Tela de inicialização do trabalho diário, registando o KM de saída e a meta de quilometragem.
3. **Registrar Abastecimento (`Página 3`):** Tela de inserção de custos, litros, captura de câmara fotográfica em formato Dropzone para guardar os recibos fiscais.
4. **Acompanhamento de Rota (`Página 4`):** Permite inserir rapidamente a quilometragem durante as entregas para manter a autonomia atualizada.
5. **Administração (`Páginas 10000+`):** Módulo administrativo nativo para gerir permissões e adicionar novos utilizadores à plataforma.

## ⚙️ Como Instalar e Testar

1. Descarregue o ficheiro de exportação da aplicação (`f206685.sql`) disponível neste repositório.
2. Acessar ao seu espaço de trabalho (Workspace) no **Oracle APEX**.
3. Navegue até ao **App Builder** e clique em **Import** (Importar).
4. Selecione o ficheiro `.sql` e siga as instruções do assistente de instalação.
5. *Nota:* Certifique-se de compilar as tabelas auxiliares (`MOT_TURNO`, `MOT_ABASTECIMENTO`, `MOT_LEITURA_KM`) no seu *SQL Workshop* caso o export não as inclua automaticamente.

## 👨‍💻 Autor

Desenvolvido para otimização de operações logísticas.
- GitHub: [@Carlos-niell](https://github.com/Carlos-niell)
