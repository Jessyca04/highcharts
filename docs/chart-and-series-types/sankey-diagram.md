{
  "chart": {
    "type": "sankey",
    "marginTop": 50
  },
  "title": {
    "text": "Composição Patrimonial - Fluxo de Fundos (Diagrama de Sankey)"
  },
  "subtitle": {
    "text": "Representação das fontes de recursos para os ativos da empresa.<br>Total Patrimônio Líquido: R$ 7.757.095,85"
  },
  "tooltip": {
    "headerFormat": "<b>{point.fromNode.name} \u2192 {point.toNode.name}</b><br>",
    "pointFormat": "{point.weight:,.2f} R$",
    "valueSuffix": " R$"
  },
  "series": [{
    "keys": ["from", "to", "weight"],
    "dataLabels": {
      "enabled": true,
      "formatter": "function() { return this.point.name + '<br>' + Highcharts.numberFormat(this.point.weight, 2, ',', '.') + ' R$'; }",
      "style": {
        "textOutline": "none",
        "fontSize": "10px"
      }
    },
    "nodes": [
      { "id": "Patrimônio Líquido" },
      { "id": "Contas a Pagar (Passivo)" },
      { "id": "Inadimplência (Passivo)" },
      { "id": "Total Ativos Brutos" },
      { "id": "Ativo: Veículos" },
      { "id": "Ativo: Máquinas e Equipamentos" },
      { "id": "Ativo: Móveis e Utensílios" },
      { "id": "Ativo: Contas a Receber" },
      { "id": "Ativo: Cash (Dólar R$ 5,55)" },
      { "id": "Ativo: Rendimentos" },
      { "id": "Ativo: Mercado Pago" },
      { "id": "Ativo: Itaú" },
      { "id": "Ativo: Bradesco" },
      { "id": "Ativo: Comodato" },
      { "id": "Ativo: Matéria-Prima" },
      { "id": "Ativo: Produto Farmpro" },
      { "id": "Ativo: Fee Agrologic" },
      { "id": "Ativo: Câmbio (Exportações a receber)" }
    ],
    "data": [
      // Links das fontes para o Total Ativos Brutos
      { "from": "Patrimônio Líquido", "to": "Total Ativos Brutos", "weight": 7757095.85 },
      { "from": "Contas a Pagar (Passivo)", "to": "Total Ativos Brutos", "weight": 3488825.35 },
      { "from": "Inadimplência (Passivo)", "to": "Total Ativos Brutos", "weight": 1300380.00 },

      // Links do Total Ativos Brutos para os Ativos Individuais
      { "from": "Total Ativos Brutos", "to": "Ativo: Veículos", "weight": 449796.91 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Máquinas e Equipamentos", "weight": 16065.21 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Móveis e Utensílios", "weight": 268582.75 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Contas a Receber", "weight": 2218164.40 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Cash (Dólar R$ 5,55)", "weight": 370740.00 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Rendimentos", "weight": 7603.95 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Mercado Pago", "weight": 20046.96 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Itaú", "weight": 199337.47 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Bradesco", "weight": 907415.83 },
      // O item 'Stone' com valor 0 foi omitido para não aparecer como um fluxo inexistente.
      { "from": "Total Ativos Brutos", "to": "Ativo: Comodato", "weight": 411900.00 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Matéria-Prima", "weight": 3670879.46 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Produto Farmpro", "weight": 2172014.90 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Fee Agrologic", "weight": 537389.54 },
      { "from": "Total Ativos Brutos", "to": "Ativo: Câmbio (Exportações a receber)", "weight": 1296363.22 }
    ]
  }]
}
