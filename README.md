<img src="https://user-images.githubusercontent.com/78829381/121952199-500cb100-cd32-11eb-9cf6-a420f6acde9e.png" width='140px' height='140px' align='left' />

# **Template para Pixel de Conversão Afilio**

Este template permite a implementação do **Pixel de Conversão Afilio** no **Google Tag Manager (GTM)**, garantindo o rastreamento correto das conversões em campanhas de **Sale** e **Lead**.

---

## **📌 Configuração**

O template possui duas configurações principais:

1. **Init** – Armazena o **Click ID** e a **origem da conversão (utm_source)** no `localStorage`.
2. **Tagging** – Dispara o **Pixel de Conversão**, incluindo os parâmetros necessários para o rastreamento.

### **🎯 Parâmetros do Pixel**

| Parâmetro                        | Descrição                                                    |
| -------------------------------- | ------------------------------------------------------------ |
| **type**                         | Tipo da campanha: `sale` (venda) ou `lead` (cadastro).       |
| **act_id**                       | ID do Pixel de Conversão (**ACT ID**).                       |
| **order_id**                     | ID único da conversão (Transaction ID, Order ID, etc.).      |
| **order_price**                  | Valor total da compra (aplicável para campanhas `sale`).     |
|**coupon**                 | Código do cupom utilizado na compra (opcional).                     |
| **adicional**                    | Define se há necessidade de um campo extra (`sim` ou `nao`). |
| **ad_xtra1 … ad_xtra5**   | Campos extras opcionais para informações adicionais.                |

---

## **📜 Permissões**

Para o correto funcionamento do template, as seguintes permissões são necessárias:

✅ **Acesso ao Local Storage e Cookies** (`afclick`, `aforigin`)  
✅ **Envio de requisições para** `https://p.afilio.com.br/`  
✅ **Leitura da URL da página**
