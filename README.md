# PROJETO_ENG_SF_IFCE
# Sistema de Controle de Estoque

 **Sistema de Controle de Estoque **. O comércio de eletrônicos lida com:
*   **Produtos de alto valor agregado:** Itens como smartphones, notebooks e consoles exigem rastreamento extremamente preciso para evitar perdas financeiras significativas.
*   **Rápida obsolescência tecnológica:** O mercado de eletrônicos é dinâmico, exigindo um controle rígido de giro para evitar que produtos desvalorizem ou fiquem obsoletos no estoque.
*   **Rastreabilidade única por lote e número de série:** Dispositivos exigem controle individualizado (como IMEI para celulares ou números de série para computadores) para fins de garantia e assistência técnica.


---

## 5. Aplicação das Boas Práticas Gerais
Com base nas melhores práticas:

### A. Documentação de Decisões Importantes
Todas as decisões arquiteturais fundamentais serão documentadas formalmente. 
*   *Exemplo prático:* Documentaremos a escolha de um **Banco de Dados Relacional (PostgreSQL)** para suportar o inventário. A justificativa técnica registrada detalhará a necessidade de suporte robusto a restrições de chave estrangeira, transações atômicas e integridade referencial — fundamentais para rastrear produtos por meio de números de série exclusivos sem risco de duplicação.

### B. Versionamento com Git
O desenvolvimento será totalmente controlado pelo Git utilizando o fluxo de ramificações (*branches*).
*   *Exemplo prático:* O repositório central terá uma branch principal estável (`main` ou `master`) [1]. Cada integrante trabalhará isolado em sua branch de funcionalidade (ex: `feature/modulo-cadastro`, `feature/justificativa-readme`) e subirá suas alterações por meio de sua própria conta [1]. A integração à branch principal só ocorrerá através de *Pull Requests* após a revisão do grupo.

### C. Padronização de Nomes e Formatação
Manteremos a coesão estética e técnica no código e na organização do projeto.
---
