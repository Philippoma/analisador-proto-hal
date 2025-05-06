
# 🔎 Analisador de Arquivos .proto, .pb e HALs (.txt)

Este notebook Colab foi desenvolvido para análise forense de arquivos do Android, com foco em:
- Arquivos `.proto` e `.pb` (Protocol Buffers)
- Arquivos de diagnóstico HAL (`.txt`) da pasta `lshal-debug`

## ✅ Funcionalidades

- Upload em lote de arquivos `.proto`, `.pb`, `.txt` e `.desc`
- Compilação automática de `.proto` com `protoc`
- Leitura e decodificação de `.pb` usando os módulos Python gerados
- Análise de arquivos HAL com identificação de falhas (`exit code`, `failed`, etc.)
- Exportação dos resultados para Excel
- Visualização gráfica de falhas detectadas
- Interface interativa com widgets (Google Colab)

## 🚀 Como usar

1. Acesse o notebook via Google Colab.
2. Faça upload de seus arquivos `.proto`, `.pb`, `.txt` usando o botão exibido.
3. Os arquivos `.proto` serão compilados automaticamente.
4. As mensagens `.pb` serão interpretadas (ajuste o nome da classe `YourMessage` no código).
5. O notebook gera um Excel `resultado_HALs_lote.xlsx` com o status dos HALs.
6. Um gráfico final mostra a distribuição de falhas detectadas.

## 📦 Requisitos

- Google Colab
- Arquivos `.proto` (com estrutura válida)
- Arquivos `.pb` (binários gerados via `protoc`)
- Arquivos HAL `.txt` exportados de dispositivos Android

## 🧠 Observações

- Substitua a linha `mensagem = pb_module.YourMessage()` pelo nome real da sua mensagem `.proto`.
- O notebook pode ser facilmente adaptado para uso local como script Python.

---

Desenvolvido com ♥ por [Seu Nome ou Equipe]
