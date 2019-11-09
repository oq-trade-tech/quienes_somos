<p align="center"><img src="oqt_logo_black_esp.png"></p>

## OQ Trading Technology
Localizados en Brooklyn, Nueva York, OQ Trading Technology es un grupo de profesionales que se especializa en conectar traders con la tecnología y plataformas de trading apropiadas. Utilizamos nuestros años de experiencia en la creación de sistemas de trading complejos para ofrecer soluciones únicas y software personalizado con el mas alto nivel de satisfacción hacia nuestros clientes.

Contact us at [info@oqtradetech.com](mailto:info@oqtradetech.com) for all inquiries.

### ¿Qué nos diferencia?
Nuestro equipo se especializa en crear o personalizar software para resolver sus necesidades únicas de trading.

### Experiencia
Opere con cualquiera de los brokers más importantes en FX (Forex) a quienes contamos como nuestros socios estratégicos. Obtenga acceso a un amplio rango de productos, incluyendo cientos de pares de monedas y CFDs.  

### Socios estratégicos
Los brokers y socios estratégicos con los que trabajamos comparten un mismo objetivo, el que usted sea exitoso.

### Disponibilidad
Estamos aquí para ayudar. Nuestro equipo se de soporte le ayudara con todas sus necesidades de trading.

### Buen servicio
Estamos aquí para servirle. Espere un alto grado de calidad en el servicio que recibirá por parte de nuestro equipo de dedicados profesionales altamente calificados.

### Costo
Nuestros precios son altamente competitivos. Trabajaremos con usted para satisfacer sus requisitos de costos.

### Tecnología
Haga su trading utilizando plataformas establecidas como MetaTrader, cTrader y Trading Station. Necesita automatización? Permita que nuestros expertos programadores codifiquen su próximo Expert Advisor en MT4 o su estrategia en LUA para los gráficos de Marketscope en TS2.

##### Código de programación de muestra

- [Trading Station II](https://github.com/oq-trade-tech/about_us#TS2-lua)
- [MetaTrader 4](https://github.com/oq-trade-tech/about_us#MT4-mq4)
- [cTrader](https://github.com/oq-trade-tech/about_us#cTrader)

#### TS2-lua
  * Código de muestra Lua

```lua
function addOrderAlert(orderID, key, data)
	if not containsKey(alertsOrder, orderID) then
		alertsOrder[orderID] = {};
	end
	alertsOrder[orderID][key] = data;
end

function addTradeAlert(tradeID, key, data)
	if not containsKey(alertsTrade, tradeID) then
		alertsTrade[tradeID] = {};
	end
	alertsTrade[tradeID][key] = data;
end

function sendAlerts()
	local messages = formatAlerts();
	if instance.parameters.advanced_alert_key ~= "" and instance.parameters.use_advanced_alert then
		sendTelegram(messages);
	end
	alertsOrder = {};
	alertsTrade = {};
end
```
#### MT4-mq4
  * Código de muestra Mq4

```lua
   for(int i = 0; i < 5; i++) {
      if(Wr[i] >= -20){
         DownArrow(40 * i + pix + 50, 120, n);
      }
      if(Wr[i] <= -80){
         UpArrow(40 * i + pix + 50, 120, n);
      }
      if((Wr[i] < -20) && (Wr[i] > -80)){
         RightArrow(40 * i + pix + 50, 120, n);
      }
      n++; 
   }
```

#### cTrader
  * C# para cTrader

```C#
	{ 
		if (TimeFrame <= TimeFrame.Hour)
    		PivotTimeFrame = TimeFrame.Daily;
    		else if (TimeFrame < TimeFrame.Daily)
    		{
    			PivotTimeFrame = TimeFrame.Weekly;
    		}
    		else
    			PivotTimeFrame = TimeFrame.Monthly;
 
 
    		Enum.TryParse(PivotColor, out pivotColor);
    		Enum.TryParse(SupportColor, out supportColor);
    		Enum.TryParse(ResistanceColor, out resistanceColor);
 
 	}
```

### Índice del sitio
* [OQT Trading Technology sitio web](https://www.oqtradetech.com)
* [OQT Trading Technology Cartera de Aplicaciones](https://oq-trade-tech.github.io)

### Equipo de liderazgo

[Marco Sierra](https://www.linkedin.com/in/marcosierra1/),
[Alejandra Diaz](https://www.linkedin.com/in/alejandra-diaz-2b973410b/)