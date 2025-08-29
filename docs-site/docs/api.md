## Funções principais


### `patologias`
```bash
patologias()
```
Função para consultar a terminologia das patologias disponíveis e seus respectivos códigos.

**Parâmetros**

- Sem parâmetros  

**Retorno**

- `string`: Tabela com as patologias e seus respectivos códigos.

---

### `deduzivel`
```bash
deduzivel(patologia: int, severidade: str, densidade: float, tipo: str)
```
Função para calcular o valor dedutível de uma patologia.

**Parâmetros**

- `patologia` (`int`): Código da patologia.
- `severidade` (`str`): Severidade (`"a"`, `"m"`, `"b"`).  
- `densidade` (`float`): Percentual de densidade.  
- `tipo` (`str`): Tipo de pavimento (`"rigido"` ou `"flexivel"`).  

**Retorno**
- `float`: Valor dedutível da patologia.

---

### `deduzivel_corrigido`
```bash
deduzivel_corrigido(dataframe: pandas.DataFrame, coluna_patologia: str, coluna_valor_deduzivel: str, tipo: str)
```
Função para calcular o valor dedutível corrigido.

**Parâmetros**

- `dataframe` (`pd.DataFrame`): Tabela com os resultados.  
- `coluna_patologia` (`str`): Nome da coluna que identifica a patologia.  
- `coluna_valor_deduzivel` (`str`): Nome da coluna com os valores dedutíveis.  
- `tipo` (`str`): Tipo de pavimento (`"rígido"` ou `"flexível"`).  

**Retorno**
- `float`: Valor dedutível corrigido total.

---