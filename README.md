# Testes de Regressão para PROCV/VLOOKUP no LibreOffice Calc

## Visão Geral
Este repositório contém arquivos de teste para verificar o funcionamento da função PROCV (VLOOKUP em inglês) no LibreOffice Calc. Os testes foram criados para o [framework de QA do LibreOffice](https://wiki.documentfoundation.org/QA) e ajudam a evitar regressões.

## Casos de Teste Incluídos
| Arquivo | Descrição |
|---------|-----------|
| `tdf_vlookup_found` | Testa busca bem-sucedida de valores |
| `tdf_vlookup_notfound` | Verifica retorno de #N/D para valores inexistentes |
| `tdf_vlookup_invalid_range` | Testa erro #REF! para intervalos inválidos |
| `tdf_vlookup_approximate` | Verifica busca aproximada |

## Como Usar
1. **Para a equipe do LibreOffice**:
   - Estes arquivos estão prontos para serem adicionados em `sc/qa/unit/data/` no código-fonte
   - Verifique o e-mail original enviado para qa@global.libreoffice.org

2. **Para teste local**:
   - Abra os arquivos `.ods` no LibreOffice Calc
   - Compare os resultados com as expectativas nos arquivos `.csv`

## Instalação
Não requer instalação - são arquivos de teste. Para integração no LibreOffice:

```bash
git clone https://github.com/lipefemoura/testes-vlookup-libreoffice-calc.git
cp contribuicao_libreoffice/*.ods /caminho/para/libreoffice/sc/qa/unit/data/ods/
cp contribuicao_libreoffice/*.csv /caminho/para/libreoffice/sc/qa/unit/data/contentCSV/
```

## Licença
MPL-2.0 ou LGPL-3.0-or-later - Veja o arquivo [LICENSE](LICENSE.md).

## Contato
Em caso de dúvidas, abra uma "Issue" neste repositório ou entre em contato com Felipe.
