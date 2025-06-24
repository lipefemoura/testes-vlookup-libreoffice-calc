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

## Status no Gerrit
Esta contribuição foi enviada ao Gerrit do LibreOffice em 24/06/2024 e está atualmente:
- [ ] Em revisão
- [x] Aprovada
- [ ] Mesclada

**Detalhes da Submissão**:
- Change-ID: Iec401964-5ee2-4616-8030-4792128f5987
- Patch Set: 1
- Branch: master
- Link: https://gerrit.libreoffice.org/c/core/+/186866

**Histórico de Revisões**:
1. **24/06/2024** - Submissão inicial
   - Adicionados 4 arquivos de teste (.ods e .csv)
   - Validação básica concluída localmente
   - [Feedback dos revisores](https://ci.libreoffice.org/job/gerrit_master_ml/43328/)

## Dependências
- Compatível com LibreOffice 7.0+
- Requer suíte de testes unitários do LibreOffice

## Licença
MPL-2.0 ou LGPL-3.0-or-later - Veja o arquivo [LICENSE](LICENSE.md).

## Contato
Para questões sobre esta contribuição:

**Autor**: Felipe Moura  
**Email**: olive.felipe2014@gmail.com  
**Gerrit**: [Felipe Moura](https://gerrit.libreoffice.org/q/owner:olive.felipe2014@gmail.com)  
**GitHub**: [@lipefemoura](https://github.com/lipefemoura)

**Canais Oficiais**:
- Lista de QA: [qa@global.libreoffice.org](mailto:qa@global.libreoffice.org)
- Bug tracker: [issues.libreoffice.org](https://bugs.documentfoundation.org)
