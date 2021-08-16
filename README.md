# SQL_CODE
This is my personal SQL ammunition. My authoral code.

(TABLE1)
CODIGO_VENDA    DATA_VENDA   CODIGO_EMPREENDIMENTO
  38523         05/01/2019        123
  38752         02/01/2019        159
  38772         08/01/2019        158
  39025         05/01/2019        652
  39035         05/01/2019        652
  39052         05/01/2019        652
  39086         03/01/2019        158
  39109         02/01/2019        158
  39184         31/01/2019        123
  39219         05/01/2019        20
  39222         05/01/2019        999
  39223         05/01/2019        159
  39230         04/01/2019        158
  39241         04/01/2019        159
  
 # Qual a quantidade de vendas por mês e por empreendimento?
 
 SELECT COUNT(CODIGO_VENDA) AS QTD_VENDAS_MES
 FROM TABLE1
 GROUP BY DATEPART(month, DATA_VENDA)

SELECT COUNT(CODIGO_VENDA) AS QTD_VENDAS_EMPREENDIMENTO
FROM TABLE1
GROUP BY CODIGO_EMPREENDIMENTO
