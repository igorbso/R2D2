# R2D2: Rapid Resort for Drug target Discovery

## Descrição

Este projeto contém um pipeline para identificar proteínas potencialmente alvo para o desenvolvimento de drogas. O pipeline utiliza diversas ferramentas de bioinformática e scripts personalizados de filtragem para comparar sequências proteicas contra bancos de dados de referência e filtrar proteínas homólogas ou não-homólogas conforme necessário.

## Estrutura do Projeto

- **R2D2.py**: Script principal que executa o pipeline completo.
- **filter.py**: Script de filtragem de proteínas homólogas contra o genoma humano.
- **filter2.py**: Script de filtragem de proteínas não-homólogas contra DEG.
- **filter3.py**: Script de filtragem de proteínas não-homólogas contra VFDB.
- **filter4.py**: Script de filtragem de proteínas não-homólogas contra DrugBank.
- **filter5.py**: Script de filtragem de proteínas homólogas contra a microbiota.

## Dependências

- Python 3
- Bibliotecas Python: `Biopython`

### Instalação de Dependências

Para instalar as dependências Python, execute:
```bash
pip install biopython
```

### Uso
Coloque o arquivo de sequência proteica de entrada no mesmo diretório.
Para executar o pipeline, utilize o seguinte comando no terminal:

```bash
python R2D2.py <arquivo_proteoma.fasta>
```

O pipeline criará uma pasta "results" e armazenará os arquivos finais nela.
