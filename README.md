# Controle B3

Os notebooks desse projeto servem para acompanhar os rendimentos das ações e fazer o imposto de renda. Basicamente, o acompanhamento das ações é feito usando o Google Spreadsheet, o que permite saber os rendimentos em "tempo real".

![spreadsheet](img/google_spreadsheet.png)

<div>
<img src="img/carteira_lucro.png" width="49%"/>
<img src="img/lucro_mes.png" width="49%"/>
</div>

## Como usar:

  É necessário baixar a planilha com as informações sobre compras e vendas de ações do site da [B3][B3]. Para isso, basta entrar no [CEI][CEI], que é o Canal Eletrônico do Investidor. Este site é gerenciado pela própria [B3][B3] e contém informações sobre seus títulos no tesouro direto, ações, CDB e etc.
   Depois de acessar a página do [CEI][CEI] é só ir em: Extratos e informativos -> Negociações de Ativos, você deve ver a opção de baixar a planilha por excel nesta página. Após isso, você deve usar o notebook ```datasets.ipynb``` para gerar os datasets que serão utiilzados pelos outros notebooks.

**O que cada notebook faz:**

  - **datasets.ipynb:** Gera o dataset que vai ser usado nos outros notebooks.
  - **Acompanhamento das ações.ipynb:** Para acompanhar a carteira de ações e gerar o google spreadsheet.
  - **Imposto de renda.ipynb:** Ajuda no imposto de renda. (Work in progress)
 
**Pacotes usados pelos notebooks:**

	- pandas        (Usado em todos)
	- numpy         (Usado em todos)
	- ipywidgets    (Para o IR)
	- matplotlib    (Para o IR e Acompanhamento)
	- seaborn       (Para o IR e Acompanhamento)
	- gspread       (Para o Acompanhamento)
	- oauth2client  (Para o Acompanhamento)

## License

See the [LICENSE](notion://www.notion.so/LICENSE.md) file for license rights and limitations (License type).

**TODO:**
  - Explicar como são adicionadas as planilhas no google.

[CEI]: https://cei.b3.com.br/CEI_Responsivo/login.aspx
[B3]: http://www.b3.com.br/pt_br/
[colab]: https://colab.research.google.com/notebooks/welcome.ipynb

## License

See the [LICENSE](LICENSE.md) file for license rights and limitations (MIT).
