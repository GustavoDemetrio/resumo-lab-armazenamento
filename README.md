# Resumo do Lab - Armazenamento no Azure

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do laboratório de **Armazenamento no Azure** na DIO.

## O que aprendi

### Criação de Conta de Armazenamento
- Nome da conta deve ter entre **3 e 24 caracteres**.
- Precisa ser **único globalmente**.
- Não aceita letras maiúsculas nem caracteres especiais.

### Tipos de Conta
- **Standard**: recomendado para a maioria dos cenários; cobrança apenas pelo uso.
- **Premium**: recomendado para cenários de **baixa latência** (mais caro, usado em aplicações críticas como PIX, bolsa de valores).

### Redundância de Armazenamento
- **LRS**: redundância local (um datacenter).
- **ZRS**: redundância de zona (múltiplas zonas de disponibilidade).
- **GRS**: redundância geográfica (região primária + secundária).
- **GZRS**: redundância de zona + geográfica.

### Armazenamento de Blobs
- **Camada Quente**: para dados acessados com frequência.
- **Camada Fria**: para dados de backup/acessados com pouca frequência.

### Configurações de Acesso
- Acesso pode ser:
  - Público (todas as redes).
  - Restrito a IPs específicos.
  - Apenas acesso privado.

### Recuperação de Dados
- Possibilidade de habilitar **recuperação de containers/blobs/arquivos**.
- Arquivos excluídos ficam salvos por um período configurado.
- Ideal para produção, não recomendado para ambientes de teste.

### Compartilhamento de Arquivos
- Feito via **SMB (\\)**, utilizando a **porta 445**.

### Filas
- Usadas para comunicação entre **aplicações** com mensagens (até 64 KB cada).

### Migração para Azure
- **Data Box Disk**: até 35 TB.
- **Data Box**: até 80 TB.
- **Data Box Heavy**: até 800 TB.
- Também é possível migrar **online** via rede.

### Ferramentas de Gerenciamento de Arquivos
- **AzCopy**: ferramenta de linha de comando para copiar/sincronizar arquivos.
  - Necessário gerar e configurar **Token de Acesso Compartilhado**.
- **Gerenciador de Armazenamento do Azure**: interface gráfica, semelhante ao Windows Explorer, compatível com Windows, MacOS e Linux.
- **Sincronização de Arquivos do Azure**: sincronização bidirecional entre arquivos locais e nuvem.

---

## Conclusão
O laboratório me permitiu entender como criar, configurar e gerenciar **contas de armazenamento no Azure**, explorando as opções de **redundância, camadas de acesso, migração de dados e ferramentas de gerenciamento**. Esse aprendizado é essencial para garantir **disponibilidade, segurança e eficiência** no uso da nuvem.

