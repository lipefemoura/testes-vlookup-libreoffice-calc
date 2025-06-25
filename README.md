# Testes de Regressão para PROCV/VLOOKUP no LibreOffice Calc

## Visão Geral
Este repositório contém arquivos de teste para verificar o funcionamento da função PROCV (VLOOKUP em inglês) no LibreOffice Calc. Os testes foram criados para o [framework de QA do LibreOffice](https://wiki.documentfoundation.org/Development/Calc_Import_Unit_Tests) e ajudam a evitar regressões.

## Casos de Teste Incluídos
| Arquivo | Descrição |
|---------|-----------|
| `tdf_vlookup_found` | Testa busca bem-sucedida de valores |
| `tdf_vlookup_notfound` | Verifica retorno de #N/D para valores inexistentes |
| `tdf_vlookup_invalid_range` | Testa erro #REF! para intervalos inválidos |
| `tdf_vlookup_approximate` | Verifica busca aproximada |

## Status no Gerrit
Esta contribuição foi enviada ao Gerrit do LibreOffice em 24/06/2024 e está atualmente:
- [x] Em revisão
- [ ] Aprovada
- [ ] Mesclada

**Detalhes da Submissão**:
- Change-ID: Iec401964-5ee2-4616-8030-4792128f5987
- Patch Set: 1
- Branch: master
- Link: https://gerrit.libreoffice.org/c/core/+/186866

**Histórico de Revisões**:
1. **23/06/2024** - Submissão inicial
   - Adicionados 4 arquivos de teste (.ods e .csv)
   - Validação básica concluída localmente
   - [Feedback dos revisores](https://ci.libreoffice.org/job/gerrit_master_ml/43328/)

## Licença
MPL-2.0 ou LGPL-3.0-or-later - Veja o arquivo [LICENSE](LICENSE.md).
